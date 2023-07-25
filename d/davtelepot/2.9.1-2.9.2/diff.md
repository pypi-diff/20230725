# Comparing `tmp/davtelepot-2.9.1.tar.gz` & `tmp/davtelepot-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "davtelepot-2.9.1.tar", last modified: Sat Apr 29 18:57:16 2023, max compression
+gzip compressed data, was "davtelepot-2.9.2.tar", last modified: Tue Jul 25 14:47:04 2023, max compression
```

## Comparing `davtelepot-2.9.1.tar` & `davtelepot-2.9.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.702412 davtelepot-2.9.1/
--rw-r--r--   0 davte     (1000) davte     (1000)       68 2018-10-23 15:20:11.000000 davtelepot-2.9.1/LICENSE
--rw-rw-r--   0 davte     (1000) davte     (1000)      153 2019-07-19 08:07:29.000000 davtelepot-2.9.1/MANIFEST.in
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-04-29 18:57:16.702412 davtelepot-2.9.1/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)     2781 2019-07-18 12:44:21.000000 davtelepot-2.9.1/README.md
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/
--rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-04-29 11:52:55.000000 davtelepot-2.9.1/davtelepot/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-04-29 15:53:32.000000 davtelepot-2.9.1/davtelepot/__main__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    70625 2022-12-12 21:45:08.000000 davtelepot-2.9.1/davtelepot/administration_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   111657 2023-04-29 15:25:02.000000 davtelepot-2.9.1/davtelepot/api.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-01-06 09:30:24.000000 davtelepot-2.9.1/davtelepot/api_helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2022-12-06 21:18:51.000000 davtelepot-2.9.1/davtelepot/authorization.py
--rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-04-29 18:02:59.000000 davtelepot-2.9.1/davtelepot/bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     8455 2023-04-29 18:55:02.000000 davtelepot-2.9.1/davtelepot/cli.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/data/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-19 07:39:50.000000 davtelepot-2.9.1/davtelepot/data/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2022-12-10 17:46:29.000000 davtelepot-2.9.1/davtelepot/database.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-11-19 14:18:50.000000 davtelepot-2.9.1/davtelepot/helper.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    16258 2019-07-18 12:44:21.000000 davtelepot-2.9.1/davtelepot/ietf_language_tags.csv
--rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/languages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    46400 2022-12-05 21:10:02.000000 davtelepot-2.9.1/davtelepot/messages.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/suggestions.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot/tools/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-06-22 20:56:16.000000 davtelepot-2.9.1/davtelepot/tools/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-06-22 20:56:16.000000 davtelepot-2.9.1/davtelepot/tools/merge_files.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2022-10-12 11:53:43.000000 davtelepot-2.9.1/davtelepot/useful_tools.py
--rw-rw-r--   0 davte     (1000) davte     (1000)    50174 2023-01-06 09:30:02.000000 davtelepot-2.9.1/davtelepot/utilities.py
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.698413 davtelepot-2.9.1/davtelepot.egg-info/
--rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/PKG-INFO
--rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/SOURCES.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/dependency_links.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/requires.txt
--rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-04-29 18:57:16.000000 davtelepot-2.9.1/davtelepot.egg-info/top_level.txt
-drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-04-29 18:57:16.702412 davtelepot-2.9.1/examples/
--rw-rw-r--   0 davte     (1000) davte     (1000)        0 2019-07-18 12:44:21.000000 davtelepot-2.9.1/examples/__init__.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-08-23 12:21:45.000000 davtelepot-2.9.1/examples/a_simple_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-08-23 12:21:45.000000 davtelepot-2.9.1/examples/more_bots_together.py
--rw-rw-r--   0 davte     (1000) davte     (1000)     3245 2020-08-23 12:11:09.000000 davtelepot-2.9.1/examples/webhook_powered_bot.py
--rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-04-29 18:57:16.702412 davtelepot-2.9.1/setup.cfg
--rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-08-23 12:11:09.000000 davtelepot-2.9.1/setup.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.160097 davtelepot-2.9.2/
+-rw-r--r--   0 davte     (1000) davte     (1000)       68 2020-01-05 17:46:41.000000 davtelepot-2.9.2/LICENSE
+-rw-r--r--   0 davte     (1000) davte     (1000)      153 2020-01-05 17:46:41.000000 davtelepot-2.9.2/MANIFEST.in
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-07-25 14:47:04.160097 davtelepot-2.9.2/PKG-INFO
+-rw-r--r--   0 davte     (1000) davte     (1000)     2781 2020-01-05 17:46:41.000000 davtelepot-2.9.2/README.md
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.156097 davtelepot-2.9.2/davtelepot/
+-rw-rw-r--   0 davte     (1000) davte     (1000)      747 2023-07-25 14:26:59.000000 davtelepot-2.9.2/davtelepot/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)      106 2023-07-25 13:31:04.000000 davtelepot-2.9.2/davtelepot/__main__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    72967 2023-07-25 14:26:13.000000 davtelepot-2.9.2/davtelepot/administration_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   111657 2023-07-25 13:38:59.000000 davtelepot-2.9.2/davtelepot/api.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10956 2023-07-25 13:28:11.000000 davtelepot-2.9.2/davtelepot/api_helper.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    31329 2023-07-25 13:28:11.000000 davtelepot-2.9.2/davtelepot/authorization.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)   143116 2023-07-25 13:38:59.000000 davtelepot-2.9.2/davtelepot/bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     8393 2023-07-25 14:42:15.000000 davtelepot-2.9.2/davtelepot/cli.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.160097 davtelepot-2.9.2/davtelepot/data/
+-rw-r--r--   0 davte     (1000) davte     (1000)        0 2020-01-05 17:46:41.000000 davtelepot-2.9.2/davtelepot/data/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3779 2023-07-25 13:28:11.000000 davtelepot-2.9.2/davtelepot/database.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     9773 2020-12-11 08:47:41.000000 davtelepot-2.9.2/davtelepot/helper.py
+-rw-r--r--   0 davte     (1000) davte     (1000)    16258 2020-01-05 17:46:41.000000 davtelepot-2.9.2/davtelepot/ietf_language_tags.csv
+-rw-rw-r--   0 davte     (1000) davte     (1000)    11316 2020-12-11 08:47:41.000000 davtelepot-2.9.2/davtelepot/languages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    48464 2023-07-25 14:26:13.000000 davtelepot-2.9.2/davtelepot/messages.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    10720 2020-12-11 08:47:41.000000 davtelepot-2.9.2/davtelepot/suggestions.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.160097 davtelepot-2.9.2/davtelepot/tools/
+-rw-rw-r--   0 davte     (1000) davte     (1000)        0 2020-07-04 17:30:12.000000 davtelepot-2.9.2/davtelepot/tools/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2543 2020-07-04 17:30:12.000000 davtelepot-2.9.2/davtelepot/tools/merge_files.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    24204 2020-12-11 08:47:41.000000 davtelepot-2.9.2/davtelepot/useful_tools.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)    50246 2023-07-25 14:36:42.000000 davtelepot-2.9.2/davtelepot/utilities.py
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.156097 davtelepot-2.9.2/davtelepot.egg-info/
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3650 2023-07-25 14:47:04.000000 davtelepot-2.9.2/davtelepot.egg-info/PKG-INFO
+-rw-rw-r--   0 davte     (1000) davte     (1000)      795 2023-07-25 14:47:04.000000 davtelepot-2.9.2/davtelepot.egg-info/SOURCES.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)        1 2023-07-25 14:47:04.000000 davtelepot-2.9.2/davtelepot.egg-info/dependency_links.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-07-25 14:47:04.000000 davtelepot-2.9.2/davtelepot.egg-info/requires.txt
+-rw-rw-r--   0 davte     (1000) davte     (1000)       20 2023-07-25 14:47:04.000000 davtelepot-2.9.2/davtelepot.egg-info/top_level.txt
+drwxrwxr-x   0 davte     (1000) davte     (1000)        0 2023-07-25 14:47:04.160097 davtelepot-2.9.2/examples/
+-rw-r--r--   0 davte     (1000) davte     (1000)        0 2020-01-05 17:46:41.000000 davtelepot-2.9.2/examples/__init__.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     6760 2020-09-26 17:25:48.000000 davtelepot-2.9.2/examples/a_simple_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)     3937 2020-09-26 17:25:48.000000 davtelepot-2.9.2/examples/more_bots_together.py
+-rw-r--r--   0 davte     (1000) davte     (1000)     3245 2020-01-05 17:46:41.000000 davtelepot-2.9.2/examples/webhook_powered_bot.py
+-rw-rw-r--   0 davte     (1000) davte     (1000)       38 2023-07-25 14:47:04.160097 davtelepot-2.9.2/setup.cfg
+-rw-rw-r--   0 davte     (1000) davte     (1000)     2237 2020-04-27 21:57:40.000000 davtelepot-2.9.2/setup.py
```

### Comparing `davtelepot-2.9.1/PKG-INFO` & `davtelepot-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.1
+Version: 2.9.2
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.1/README.md` & `davtelepot-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/__init__.py` & `davtelepot-2.9.2/davtelepot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     ```
 """
 
 __author__ = "Davide Testa"
 __email__ = "davide@davte.it"
 __credits__ = ["Marco Origlia", "Nick Lee @Nickoala"]
 __license__ = "GNU General Public License v3.0"
-__version__ = "2.9.1"
+__version__ = "2.9.2"
 __maintainer__ = "Davide Testa"
 __contact__ = "t.me/davte"
 
 from davtelepot import (administration_tools, api, authorization,
                         bot, helper, languages, messages, suggestions,
                         useful_tools, utilities)
```

### Comparing `davtelepot-2.9.1/davtelepot/administration_tools.py` & `davtelepot-2.9.2/davtelepot/administration_tools.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,21 +25,25 @@
 # Project modules
 from davtelepot.messages import default_admin_messages, default_talk_messages
 from davtelepot.bot import Bot
 from davtelepot.utilities import (
     async_wrapper, CachedPage, Confirmator, extract, get_cleaned_text,
     get_user, clean_html_string, line_drawing_unordered_list, make_button,
     make_inline_keyboard, remove_html_tags, send_part_of_text_file,
-    send_csv_file, make_lines_of_buttons
+    send_csv_file, make_lines_of_buttons, join_path
 )
 
 # Use this parameter in SQL `LIMIT x OFFSET y` clauses
 rows_number_limit = 10
 
 command_description_parser = re.compile(r'(?P<command>\w+)(\s?-\s?(?P<description>.*))?')
+variable_regex = re.compile(r"(?P<name>[a-zA-Z][\w]*)\s*=\s*"
+                            r"(?P<value>[\d.,]+|True|False|"
+                            r"'[^']*'|"
+                            r"\"[^\"]*\")")
 
 
 async def _forward_to(update,
                       bot: Bot,
                       sender,
                       addressee,
                       is_admin=False):
@@ -1801,14 +1805,48 @@
                 text=text,
                 reply_markup=reply_markup
             )
         )
     return result
 
 
+async def _config_command(bot: Bot, update: dict,
+                          user_record: dict, language: str):
+    text = get_cleaned_text(
+        update,
+        bot,
+        ['config']
+    )
+    if not text:
+        return bot.get_message('admin', 'config_command',
+                               'instructions',
+                               user_record=user_record,
+                               language=language)
+    match = variable_regex.match(text)
+    if not match:
+        return bot.get_message('admin', 'config_command',
+                               'invalid_input',
+                               user_record=user_record,
+                               language=language)
+    match = match.groupdict()
+    if (',' in match['value']
+            and not match['value'].startswith('\'')
+            and not match['value'].startswith('"')):
+        match['value'] = match['value'].replace(',', '.')
+    new_variable = f"{match['name']} = {match['value']}"
+    with open(join_path(bot.path, 'data', 'config.py'),
+              'a') as configuration_file:
+        configuration_file.write(f"{new_variable}\n")
+    return bot.get_message('admin', 'config_command',
+                           'success',
+                           new_variable=new_variable,
+                           user_record=user_record,
+                           language=language)
+
+
 def init(telegram_bot: Bot,
          talk_messages: dict = None,
          admin_messages: dict = None,
          packages: List[types.ModuleType] = None):
     """Assign parsers, commands, buttons and queries to given `bot`."""
     if packages is None:
         packages = []
@@ -2015,7 +2053,22 @@
                           show_in_keyboard=False,
                           authorization_level='admin')
     async def version_command(bot, update, user_record, language):
         return await _version_command(bot=bot,
                                       update=update,
                                       user_record=user_record,
                                       language=language)
+
+    @telegram_bot.command(command='/config',
+                          aliases=[],
+                          **{key: admin_messages['config_command'][key]
+                             for key in ('reply_keyboard_button',
+                                         'description',
+                                         'help_section',)
+                             },
+                          show_in_keyboard=False,
+                          authorization_level='admin')
+    async def config_command(bot, update, user_record, language):
+        return await _config_command(bot=bot,
+                                     update=update,
+                                     user_record=user_record,
+                                     language=language)
```

### Comparing `davtelepot-2.9.1/davtelepot/api.py` & `davtelepot-2.9.2/davtelepot/api.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/api_helper.py` & `davtelepot-2.9.2/davtelepot/api_helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/authorization.py` & `davtelepot-2.9.2/davtelepot/authorization.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/bot.py` & `davtelepot-2.9.2/davtelepot/bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/cli.py` & `davtelepot-2.9.2/davtelepot/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,18 @@
 from typing import Any, Dict, Union
 
 import davtelepot.authorization as authorization
 import davtelepot.administration_tools as administration_tools
 import davtelepot.helper as helper
 from davtelepot.bot import Bot
 from davtelepot.utilities import (get_cleaned_text, get_secure_key,
-                                  get_user, json_read, json_write,
+                                  get_user, join_path, json_read, json_write,
                                   line_drawing_unordered_list)
 
 
-def join_path(*args):
-    return os.path.abspath(os.path.join(*args))
-
-
 def dir_path(path):
     if os.path.isdir(path) and os.access(path, os.W_OK):
         return path
     else:
         raise argparse.ArgumentTypeError(f"`{path}` is not a valid path")
 
 
@@ -95,19 +91,21 @@
         return "👑 You have been granted full powers! 👑"
     else:
         print(f"The secret entered (`{text}`) is wrong. Enter `{secret}` instead.")
 
 
 def allow_elevation_to_admin(telegram_bot: Bot) -> None:
     secret = get_secure_key(length=15)
+
     @telegram_bot.additional_task('BEFORE')
     async def print_secret():
         await telegram_bot.get_me()
         logging.info(f"To get administration privileges, enter code {secret} "
                      f"or click here: https://t.me/{telegram_bot.name}?start=00elevate_{secret}")
+
     @telegram_bot.command(command='/elevate', aliases=['00elevate_'], show_in_keyboard=False,
                           authorization_level='anybody')
     async def _elevate_to_admin(bot, update, user_record):
         return await elevate_to_admin(bot=bot, update=update,
                                       user_record=user_record,
                                       secret=secret)
     return
@@ -139,15 +137,15 @@
         if len(records) == 1 and offset == 0:
             break
         last_text = text
         print("=== Users ===",
               line_drawing_unordered_list(
                   list(map(lambda x: get_user(x, False),
                            records[:max_shown]))
-                  + (['...'] if len(records)>=max_shown else [])
+                  + (['...'] if len(records) >= max_shown else [])
               ),
               sep='\n')
         text = input("Select a recipient: write part of their name.\t\t")
     while True:
         text = input(f"Write a message for {get_user(records[0], False)}\t\t")
         if input("Should I send it? Y to send, anything else cancel\t\t").lower() == "y":
             break
@@ -161,15 +159,15 @@
 
 
 def run_from_command_line():
     arguments = get_cli_arguments()
     stored_arguments_file = os.path.join(arguments['path'],
                                          'cli_args.json')
     for key, value in json_read(file_=stored_arguments_file,
-                                     default={}).items():
+                                default={}).items():
         if key not in arguments or not arguments[key]:
             arguments[key] = value
     set_loggers(**{k: v
                    for k, v in arguments.items()
                    if k in ('log_file', 'error_log_file')})
     if 'error_log_file' in arguments:
         Bot.set_class_errors_file_path(file_path=arguments['error_log_file'])
```

### Comparing `davtelepot-2.9.1/davtelepot/database.py` & `davtelepot-2.9.2/davtelepot/database.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/helper.py` & `davtelepot-2.9.2/davtelepot/helper.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/ietf_language_tags.csv` & `davtelepot-2.9.2/davtelepot/ietf_language_tags.csv`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/languages.py` & `davtelepot-2.9.2/davtelepot/languages.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/messages.py` & `davtelepot-2.9.2/davtelepot/messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,61 @@
             'it': "↩️ Operazione annullata",
         },
         'lower': {
             'en': "cancel",
             'it': "annulla",
         },
     },
+    'config_command': {
+        'description': {
+            'en': "Add a variable to the configuration file",
+            'it': "Aggiungi una variabile al file di configurazione",
+        },
+        'help_section': None,
+        'instructions': {
+            'en': "<b>Config 🔧</b>\n\n"
+                  "<i>Send me a new configuration variable, for example:</i>\n"
+                  "<code>variable = 2</code>",
+            'it': "<b>Configurazione 🔧</b>\n\n"
+                  "<i>Mandami una variabile da aggiungere al file di "
+                  "configurazione, per esempio:</i>\n"
+                  "<code>variabile = 2</code>",
+        },
+        'invalid_input': {
+            'en': "<b>❌ Invalid input 🔧</b>\n\n"
+                  "<i>Send me a new configuration variable, for example:</i>\n"
+                  "<code>int_var = 2\n"
+                  "str_var = 'test'\n"
+                  "bool_var = False\n"
+                  "float_var = 3.5</code>",
+            'it': "<b>❌ Configurazione scorretta 🔧</b>\n\n"
+                  "<i>Mandami una variabile da aggiungere al file di "
+                  "configurazione, per esempio:</i>\n"
+                  "<code>var_int = 2\n"
+                  "var_str = 'test'\n"
+                  "var_bool = False\n"
+                  "var_float = 3.5</code>",
+        },
+        'reply_keyboard_button': {
+            'en': "Config 🔧",
+            'it': "Configurazione 🔧",
+        },
+        'success': {
+            'en': "<b>✔️ Configuration updated 🔧</b>\n\n"
+                  "The following variable has been added to the configuration "
+                  "file:\n"
+                  "<code>{new_variable}</code>\n\n"
+                  "/restart to apply",
+            'it': "<b>✔️ Configurazione aggiornata 🔧</b>\n\n"
+                  "La seguente variabile è stata aggiunta al file di "
+                  "configurazione:\n"
+                  "<code>{new_variable}</code>\n\n"
+                  "Per rendere effettive le modifiche fai /restart",
+        },
+    },
     'confirm': {
         'en': "🔄 Click again to confirm",
         'it': "🔄 Clicka di nuovo per confermare",
     },
     'db_command': {
         'db_sent': {
             'en': "Database sent.",
```

### Comparing `davtelepot-2.9.1/davtelepot/suggestions.py` & `davtelepot-2.9.2/davtelepot/suggestions.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/tools/merge_files.py` & `davtelepot-2.9.2/davtelepot/tools/merge_files.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/useful_tools.py` & `davtelepot-2.9.2/davtelepot/useful_tools.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/davtelepot/utilities.py` & `davtelepot-2.9.2/davtelepot/utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1734,7 +1734,11 @@
             "Exception {e}:\n{o}\n{er}".format(
                 e=e,
                 o=(stdout.decode().strip() if stdout else ''),
                 er=(stderr.decode().strip() if stderr else '')
             )
         )
     return stdout, stderr
+
+
+def join_path(*args):
+    return os.path.abspath(os.path.join(*args))
```

### Comparing `davtelepot-2.9.1/davtelepot.egg-info/PKG-INFO` & `davtelepot-2.9.2/davtelepot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: davtelepot
-Version: 2.9.1
+Version: 2.9.2
 Summary: Telegram bot API mirroring class, featuring dataset-powered SQLite databases.
 Home-page: https://gogs.davte.it/davte/davtelepot
 Author: Davide Testa
 Author-email: davide@davte.it
 License: GNU General Public License v3.0
 Keywords: telegram bot python asyncio async aiohttp
 Platform: any
```

### Comparing `davtelepot-2.9.1/davtelepot.egg-info/SOURCES.txt` & `davtelepot-2.9.2/davtelepot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/examples/a_simple_bot.py` & `davtelepot-2.9.2/examples/a_simple_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/examples/more_bots_together.py` & `davtelepot-2.9.2/examples/more_bots_together.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/examples/webhook_powered_bot.py` & `davtelepot-2.9.2/examples/webhook_powered_bot.py`

 * *Files identical despite different names*

### Comparing `davtelepot-2.9.1/setup.py` & `davtelepot-2.9.2/setup.py`

 * *Files identical despite different names*

