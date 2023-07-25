# Comparing `tmp/emoji-2.6.0.tar.gz` & `tmp/emoji-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emoji-2.6.0.tar", last modified: Wed Jun 28 09:02:12 2023, max compression
+gzip compressed data, was "emoji-2.7.0.tar", last modified: Tue Jul 25 07:47:44 2023, max compression
```

## Comparing `emoji-2.6.0.tar` & `emoji-2.7.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-06-28 09:02:12.315892 emoji-2.6.0/
--rw-r--r--   0 tahir      (501) staff       (20)     4309 2023-06-28 08:51:40.000000 emoji-2.6.0/CHANGES.md
--rw-r--r--   0 tahir      (501) staff       (20)     1483 2023-06-08 08:36:57.000000 emoji-2.6.0/LICENSE.txt
--rw-r--r--   0 tahir      (501) staff       (20)      142 2023-05-24 12:55:25.000000 emoji-2.6.0/MANIFEST.in
--rw-r--r--   0 tahir      (501) staff       (20)     5157 2023-06-28 09:02:12.315989 emoji-2.6.0/PKG-INFO
--rw-r--r--   0 tahir      (501) staff       (20)     3817 2023-06-08 08:34:25.000000 emoji-2.6.0/README.rst
-drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-06-28 09:02:12.305486 emoji-2.6.0/emoji/
--rw-r--r--   0 tahir      (501) staff       (20)     2358 2023-06-28 08:51:40.000000 emoji-2.6.0/emoji/__init__.py
--rw-r--r--   0 tahir      (501) staff       (20)      929 2023-06-08 08:34:25.000000 emoji-2.6.0/emoji/__init__.pyi
--rw-r--r--   0 tahir      (501) staff       (20)    13860 2023-06-28 08:51:40.000000 emoji-2.6.0/emoji/core.py
--rw-r--r--   0 tahir      (501) staff       (20)     1310 2023-06-08 08:34:25.000000 emoji-2.6.0/emoji/core.pyi
--rw-r--r--   0 tahir      (501) staff       (20)        0 2023-05-24 12:55:25.000000 emoji-2.6.0/emoji/py.typed
--rw-r--r--   0 tahir      (501) staff       (20)    11876 2023-06-15 17:34:39.000000 emoji-2.6.0/emoji/tokenizer.py
--rw-r--r--   0 tahir      (501) staff       (20)     1201 2023-06-08 08:34:25.000000 emoji-2.6.0/emoji/tokenizer.pyi
-drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-06-28 09:02:12.310639 emoji-2.6.0/emoji/unicode_codes/
--rw-r--r--   0 tahir      (501) staff       (20)     1291 2023-06-08 08:34:25.000000 emoji-2.6.0/emoji/unicode_codes/__init__.py
--rw-r--r--   0 tahir      (501) staff       (20)      243 2023-05-24 12:55:25.000000 emoji-2.6.0/emoji/unicode_codes/__init__.pyi
--rw-r--r--   0 tahir      (501) staff       (20)  2919285 2023-06-08 14:53:57.000000 emoji-2.6.0/emoji/unicode_codes/data_dict.py
--rw-r--r--   0 tahir      (501) staff       (20)      155 2023-05-24 12:55:25.000000 emoji-2.6.0/emoji/unicode_codes/data_dict.pyi
--rw-r--r--   0 tahir      (501) staff       (20)        0 2023-05-24 12:55:25.000000 emoji-2.6.0/emoji/unicode_codes/py.typed
-drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-06-28 09:02:12.306366 emoji-2.6.0/emoji.egg-info/
--rw-r--r--   0 tahir      (501) staff       (20)     5157 2023-06-28 09:02:12.000000 emoji-2.6.0/emoji.egg-info/PKG-INFO
--rw-r--r--   0 tahir      (501) staff       (20)      734 2023-06-28 09:02:12.000000 emoji-2.6.0/emoji.egg-info/SOURCES.txt
--rw-r--r--   0 tahir      (501) staff       (20)        1 2023-06-28 09:02:12.000000 emoji-2.6.0/emoji.egg-info/dependency_links.txt
--rw-r--r--   0 tahir      (501) staff       (20)       33 2023-06-28 09:02:12.000000 emoji-2.6.0/emoji.egg-info/requires.txt
--rw-r--r--   0 tahir      (501) staff       (20)        6 2023-06-28 09:02:12.000000 emoji-2.6.0/emoji.egg-info/top_level.txt
--rw-r--r--   0 tahir      (501) staff       (20)        1 2023-05-24 12:55:46.000000 emoji-2.6.0/emoji.egg-info/zip-safe
--rw-r--r--   0 tahir      (501) staff       (20)      107 2023-06-28 09:02:12.316230 emoji-2.6.0/setup.cfg
--rw-r--r--   0 tahir      (501) staff       (20)     2674 2023-06-08 08:34:25.000000 emoji-2.6.0/setup.py
-drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-06-28 09:02:12.315677 emoji-2.6.0/tests/
--rw-r--r--   0 tahir      (501) staff       (20)       45 2023-06-08 08:34:25.000000 emoji-2.6.0/tests/__init__.py
--rw-r--r--   0 tahir      (501) staff       (20)     4997 2023-06-15 17:34:39.000000 emoji-2.6.0/tests/test_analyze.py
--rw-r--r--   0 tahir      (501) staff       (20)    26522 2023-06-28 08:51:40.000000 emoji-2.6.0/tests/test_core.py
--rw-r--r--   0 tahir      (501) staff       (20)     1739 2023-06-08 14:53:57.000000 emoji-2.6.0/tests/test_dict.py
--rw-r--r--   0 tahir      (501) staff       (20)     2139 2023-06-08 14:53:57.000000 emoji-2.6.0/tests/test_nfkc.py
--rw-r--r--   0 tahir      (501) staff       (20)     1355 2023-06-08 08:34:25.000000 emoji-2.6.0/tests/test_unicode_codes.py
--rw-r--r--   0 tahir      (501) staff       (20)     3522 2023-06-08 14:53:57.000000 emoji-2.6.0/tests/test_versions.py
--rw-r--r--   0 tahir      (501) staff       (20)     7928 2023-06-15 17:34:39.000000 emoji-2.6.0/tests/test_zwj_common.py
--rw-r--r--   0 tahir      (501) staff       (20)     6489 2023-06-08 14:53:57.000000 emoji-2.6.0/tests/test_zwj_keep.py
--rw-r--r--   0 tahir      (501) staff       (20)     5502 2023-06-08 14:53:57.000000 emoji-2.6.0/tests/test_zwj_remove.py
+drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-07-25 07:47:44.111787 emoji-2.7.0/
+-rw-r--r--   0 tahir      (501) staff       (20)     4483 2023-07-25 07:47:23.000000 emoji-2.7.0/CHANGES.md
+-rw-r--r--   0 tahir      (501) staff       (20)     1483 2023-06-08 08:36:57.000000 emoji-2.7.0/LICENSE.txt
+-rw-r--r--   0 tahir      (501) staff       (20)      142 2023-05-24 12:55:25.000000 emoji-2.7.0/MANIFEST.in
+-rw-r--r--   0 tahir      (501) staff       (20)     5157 2023-07-25 07:47:44.111900 emoji-2.7.0/PKG-INFO
+-rw-r--r--   0 tahir      (501) staff       (20)     3817 2023-06-08 08:34:25.000000 emoji-2.7.0/README.rst
+drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-07-25 07:47:44.102686 emoji-2.7.0/emoji/
+-rw-r--r--   0 tahir      (501) staff       (20)     2358 2023-07-25 07:47:23.000000 emoji-2.7.0/emoji/__init__.py
+-rw-r--r--   0 tahir      (501) staff       (20)      929 2023-06-08 08:34:25.000000 emoji-2.7.0/emoji/__init__.pyi
+-rw-r--r--   0 tahir      (501) staff       (20)    13860 2023-06-28 08:51:40.000000 emoji-2.7.0/emoji/core.py
+-rw-r--r--   0 tahir      (501) staff       (20)     1310 2023-06-08 08:34:25.000000 emoji-2.7.0/emoji/core.pyi
+-rw-r--r--   0 tahir      (501) staff       (20)        0 2023-05-24 12:55:25.000000 emoji-2.7.0/emoji/py.typed
+-rw-r--r--   0 tahir      (501) staff       (20)    11876 2023-06-15 17:34:39.000000 emoji-2.7.0/emoji/tokenizer.py
+-rw-r--r--   0 tahir      (501) staff       (20)     1201 2023-06-08 08:34:25.000000 emoji-2.7.0/emoji/tokenizer.pyi
+drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-07-25 07:47:44.107590 emoji-2.7.0/emoji/unicode_codes/
+-rw-r--r--   0 tahir      (501) staff       (20)     1291 2023-06-08 08:34:25.000000 emoji-2.7.0/emoji/unicode_codes/__init__.py
+-rw-r--r--   0 tahir      (501) staff       (20)      243 2023-05-24 12:55:25.000000 emoji-2.7.0/emoji/unicode_codes/__init__.pyi
+-rw-r--r--   0 tahir      (501) staff       (20)  2979081 2023-07-25 07:38:59.000000 emoji-2.7.0/emoji/unicode_codes/data_dict.py
+-rw-r--r--   0 tahir      (501) staff       (20)      155 2023-05-24 12:55:25.000000 emoji-2.7.0/emoji/unicode_codes/data_dict.pyi
+-rw-r--r--   0 tahir      (501) staff       (20)        0 2023-05-24 12:55:25.000000 emoji-2.7.0/emoji/unicode_codes/py.typed
+drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-07-25 07:47:44.103571 emoji-2.7.0/emoji.egg-info/
+-rw-r--r--   0 tahir      (501) staff       (20)     5157 2023-07-25 07:47:44.000000 emoji-2.7.0/emoji.egg-info/PKG-INFO
+-rw-r--r--   0 tahir      (501) staff       (20)      749 2023-07-25 07:47:44.000000 emoji-2.7.0/emoji.egg-info/SOURCES.txt
+-rw-r--r--   0 tahir      (501) staff       (20)        1 2023-07-25 07:47:44.000000 emoji-2.7.0/emoji.egg-info/dependency_links.txt
+-rw-r--r--   0 tahir      (501) staff       (20)       33 2023-07-25 07:47:44.000000 emoji-2.7.0/emoji.egg-info/requires.txt
+-rw-r--r--   0 tahir      (501) staff       (20)        6 2023-07-25 07:47:44.000000 emoji-2.7.0/emoji.egg-info/top_level.txt
+-rw-r--r--   0 tahir      (501) staff       (20)        1 2023-05-24 12:55:46.000000 emoji-2.7.0/emoji.egg-info/zip-safe
+-rw-r--r--   0 tahir      (501) staff       (20)       98 2023-07-25 07:38:59.000000 emoji-2.7.0/pyproject.toml
+-rw-r--r--   0 tahir      (501) staff       (20)      107 2023-07-25 07:47:44.112187 emoji-2.7.0/setup.cfg
+-rw-r--r--   0 tahir      (501) staff       (20)     2674 2023-06-08 08:34:25.000000 emoji-2.7.0/setup.py
+drwxr-xr-x   0 tahir      (501) staff       (20)        0 2023-07-25 07:47:44.111506 emoji-2.7.0/tests/
+-rw-r--r--   0 tahir      (501) staff       (20)       45 2023-06-08 08:34:25.000000 emoji-2.7.0/tests/__init__.py
+-rw-r--r--   0 tahir      (501) staff       (20)     4997 2023-06-15 17:34:39.000000 emoji-2.7.0/tests/test_analyze.py
+-rw-r--r--   0 tahir      (501) staff       (20)    26522 2023-07-25 07:38:59.000000 emoji-2.7.0/tests/test_core.py
+-rw-r--r--   0 tahir      (501) staff       (20)     1739 2023-06-08 14:53:57.000000 emoji-2.7.0/tests/test_dict.py
+-rw-r--r--   0 tahir      (501) staff       (20)     2139 2023-06-08 14:53:57.000000 emoji-2.7.0/tests/test_nfkc.py
+-rw-r--r--   0 tahir      (501) staff       (20)     1355 2023-06-08 08:34:25.000000 emoji-2.7.0/tests/test_unicode_codes.py
+-rw-r--r--   0 tahir      (501) staff       (20)     3522 2023-06-08 14:53:57.000000 emoji-2.7.0/tests/test_versions.py
+-rw-r--r--   0 tahir      (501) staff       (20)     7928 2023-06-15 17:34:39.000000 emoji-2.7.0/tests/test_zwj_common.py
+-rw-r--r--   0 tahir      (501) staff       (20)     6489 2023-06-08 14:53:57.000000 emoji-2.7.0/tests/test_zwj_keep.py
+-rw-r--r--   0 tahir      (501) staff       (20)     5502 2023-06-08 14:53:57.000000 emoji-2.7.0/tests/test_zwj_remove.py
```

### Comparing `emoji-2.6.0/CHANGES.md` & `emoji-2.7.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 emoji
 =====
 
+v2.7.0 (2023-07-25)
+-----
+* Extract aliases from cheat sheet and youtube
+* Fix extracting translations from emojiterra
+* Update EMOJI_DATA with new aliases and translations
+
 v2.6.0 (2023-06-28)
 -----
 * Added new function purely_emoji() | Check if a string contains only emojis
 
 v2.5.1 (2023-06-15)
 -----
 * Fix Malformed zero width joiner (\u200d) causes IndexError
```

### Comparing `emoji-2.6.0/LICENSE.txt` & `emoji-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/PKG-INFO` & `emoji-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emoji
-Version: 2.6.0
+Version: 2.7.0
 Summary: Emoji for Python
 Home-page: https://github.com/carpedm20/emoji/
 Author: Taehoon Kim, Kevin Wurster
 Author-email: carpedm20@gmail.com
 License: New BSD
 Keywords: emoji
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `emoji-2.6.0/README.rst` & `emoji-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/__init__.py` & `emoji-2.7.0/emoji/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     'emoji_list', 'distinct_emoji_list', 'emoji_count',
     'replace_emoji', 'is_emoji', 'purely_emoji', 'version',
     'Token', 'EmojiMatch', 'EmojiMatchZWJ', 'EmojiMatchZWJNonRGI',
     # emoji.unicode_codes
     'EMOJI_DATA', 'STATUS', 'LANGUAGES',
 ]
 
-__version__ = '2.6.0'
+__version__ = '2.7.0'
 __author__ = 'Taehoon Kim, Kevin Wurster'
 __email__ = 'carpedm20@gmail.com'
 # and wursterk@gmail.com, tahir.jalilov@gmail.com
 __source__ = 'https://github.com/carpedm20/emoji/'
 __license__ = '''
 New BSD License
```

### Comparing `emoji-2.6.0/emoji/__init__.pyi` & `emoji-2.7.0/emoji/__init__.pyi`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/core.py` & `emoji-2.7.0/emoji/core.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/core.pyi` & `emoji-2.7.0/emoji/core.pyi`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/tokenizer.py` & `emoji-2.7.0/emoji/tokenizer.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/tokenizer.pyi` & `emoji-2.7.0/emoji/tokenizer.pyi`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/unicode_codes/__init__.py` & `emoji-2.7.0/emoji/unicode_codes/__init__.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/emoji/unicode_codes/data_dict.py` & `emoji-2.7.0/emoji/unicode_codes/data_dict.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         'id': ':medali_perunggu:',
         'zh': ':铜牌:'
     },
     '\U0001F18E': {  # 🆎
         'en': ':AB_button_(blood_type):',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':ab:'],
+        'alias': [':ab:', ':ab_button_blood_type:'],
         'de': ':großbuchstaben_ab_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_ab:',
         'fr': ':groupe_sanguin_ab:',
         'ja': ':血液型ab型:',
         'ko': ':에이비형:',
         'pt': ':botão_ab_(tipo_sanguíneo):',
         'it': ':gruppo_sanguigno_ab:',
@@ -105,15 +105,15 @@
         'id': ':tombol_ab_(golongan_darah):',
         'zh': ':AB型血:'
     },
     '\U0001F3E7': {  # 🏧
         'en': ':ATM_sign:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':atm:'],
+        'alias': [':atm:', ':atm_sign:'],
         'de': ':symbol_geldautomat:',
         'es': ':señal_de_cajero_automático:',
         'fr': ':distributeur_de_billets:',
         'ja': ':atm:',
         'ko': ':에이티엠:',
         'pt': ':símbolo_de_caixa_automático:',
         'it': ':simbolo_dello_sportello_bancomat:',
@@ -121,15 +121,15 @@
         'id': ':tanda_atm:',
         'zh': ':取款机:'
     },
     '\U0001F170\U0000FE0F': {  # 🅰️
         'en': ':A_button_(blood_type):',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':a:'],
+        'alias': [':a:', ':a_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_a_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_a:',
         'fr': ':groupe_sanguin_a:',
         'ja': ':血液型a型:',
         'ko': ':에이형:',
         'pt': ':botão_a_(tipo_sanguíneo):',
@@ -138,15 +138,15 @@
         'id': ':tombol_a_(golongan_darah):',
         'zh': ':A型血:'
     },
     '\U0001F170': {  # 🅰
         'en': ':A_button_(blood_type):',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':a:'],
+        'alias': [':a:', ':a_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_a_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_a:',
         'fr': ':groupe_sanguin_a:',
         'ja': ':血液型a型:',
         'ko': ':에이형:',
         'pt': ':botão_a_(tipo_sanguíneo):',
@@ -445,15 +445,15 @@
         'id': ':bendera_azerbaijan:',
         'zh': ':阿塞拜疆:'
     },
     '\U0001F519': {  # 🔙
         'en': ':BACK_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':back:'],
+        'alias': [':back:', ':back_arrow:'],
         'de': ':back-pfeil:',
         'es': ':flecha_back:',
         'fr': ':flèche_retour:',
         'ja': ':back矢印:',
         'ko': ':뒤로:',
         'pt': ':seta_back:',
         'it': ':freccia_back:',
@@ -461,15 +461,15 @@
         'id': ':tanda_panah_back:',
         'zh': ':返回箭头:'
     },
     '\U0001F171\U0000FE0F': {  # 🅱️
         'en': ':B_button_(blood_type):',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':b:'],
+        'alias': [':b:', ':b_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_b_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_b:',
         'fr': ':groupe_sanguin_b:',
         'ja': ':血液型b型:',
         'ko': ':비형:',
         'pt': ':botão_b_(tipo_sanguíneo):',
@@ -478,15 +478,15 @@
         'id': ':tombol_b_(golongan_darah):',
         'zh': ':B型血:'
     },
     '\U0001F171': {  # 🅱
         'en': ':B_button_(blood_type):',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':b:'],
+        'alias': [':b:', ':b_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_b_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_b:',
         'fr': ':groupe_sanguin_b:',
         'ja': ':血液型b型:',
         'ko': ':비형:',
         'pt': ':botão_b_(tipo_sanguíneo):',
@@ -831,15 +831,15 @@
         'id': ':bendera_burundi:',
         'zh': ':布隆迪:'
     },
     '\U0001F191': {  # 🆑
         'en': ':CL_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':cl:'],
+        'alias': [':cl:', ':cl_button:'],
         'de': ':großbuchstaben_cl_in_rotem_quadrat:',
         'es': ':borrar:',
         'fr': ':bouton_effacer:',
         'ja': ':clマーク:',
         'ko': ':씨엘:',
         'pt': ':botão_cl:',
         'it': ':pulsante_cl:',
@@ -847,15 +847,15 @@
         'id': ':tombol_cl:',
         'zh': ':CL按钮:'
     },
     '\U0001F192': {  # 🆒
         'en': ':COOL_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':cool:'],
+        'alias': [':cool:', ':cool_button:'],
         'de': ':wort_cool_in_blauem_quadrat:',
         'es': ':botón_cool:',
         'fr': ':bouton_cool:',
         'ja': ':coolマーク:',
         'ko': ':쿨:',
         'pt': ':botão_cool:',
         'it': ':pulsante_cool:',
@@ -1425,15 +1425,15 @@
         'id': ':bendera_republik_dominika:',
         'zh': ':多米尼加共和国:'
     },
     '\U0001F51A': {  # 🔚
         'en': ':END_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':end:'],
+        'alias': [':end:', ':end_arrow:'],
         'de': ':end-pfeil:',
         'es': ':flecha_end:',
         'fr': ':flèche_fin:',
         'ja': ':end矢印:',
         'ko': ':종료:',
         'pt': ':seta_end:',
         'it': ':freccia_end:',
@@ -1601,15 +1601,15 @@
         'id': ':bendera_uni_eropa:',
         'zh': ':欧盟:'
     },
     '\U0001F193': {  # 🆓
         'en': ':FREE_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':free:'],
+        'alias': [':free:', ':free_button:'],
         'de': ':wort_free_in_blauem_quadrat:',
         'es': ':botón_free:',
         'fr': ':bouton_gratuit:',
         'ja': ':freeマーク:',
         'ko': ':프리:',
         'pt': ':botão_free:',
         'it': ':pulsante_free:',
@@ -2098,15 +2098,15 @@
         'id': ':bendera_hungaria:',
         'zh': ':匈牙利:'
     },
     '\U0001F194': {  # 🆔
         'en': ':ID_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':id:'],
+        'alias': [':id:', ':id_button:'],
         'de': ':großbuchstaben_id_in_lila_quadrat:',
         'es': ':símbolo_de_identificación:',
         'fr': ':bouton_identifiant:',
         'ja': ':idマーク:',
         'ko': ':아이디:',
         'pt': ':botão_id:',
         'it': ':pulsante_id:',
@@ -2290,15 +2290,15 @@
         'id': ':bendera_jepang:',
         'zh': ':日本:'
     },
     '\U0001F251': {  # 🉑
         'en': ':Japanese_acceptable_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':accept:'],
+        'alias': [':accept:', ':japanese_acceptable_button:'],
         'de': ':schriftzeichen_für_akzeptieren:',
         'es': ':ideograma_japonés_para_aceptable:',
         'fr': ':bouton_accepter_en_japonais:',
         'ja': ':可マーク:',
         'ko': ':옳을_가:',
         'pt': ':botão_japonês_de_“aceitável”:',
         'it': ':ideogramma_giapponese_di_“accettabile”:',
@@ -2306,15 +2306,15 @@
         'id': ':tombol_jepang_dapat_diterima:',
         'zh': ':可:'
     },
     '\U0001F238': {  # 🈸
         'en': ':Japanese_application_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u7533:'],
+        'alias': [':u7533:', ':japanese_application_button:'],
         'de': ':schriftzeichen_für_anwenden:',
         'es': ':ideograma_japonés_para_aplicación:',
         'fr': ':bouton_application_en_japonais:',
         'ja': ':申マーク:',
         'ko': ':거듭_신:',
         'pt': ':botão_japonês_de_“aplicação”:',
         'it': ':ideogramma_giapponese_di_“candidatura”:',
@@ -2322,15 +2322,15 @@
         'id': ':tombol_jepang_lamaran_kerja:',
         'zh': ':申:'
     },
     '\U0001F250': {  # 🉐
         'en': ':Japanese_bargain_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':ideograph_advantage:'],
+        'alias': [':ideograph_advantage:', ':japanese_bargain_button:'],
         'de': ':schriftzeichen_für_schnäppchen:',
         'es': ':ideograma_japonés_para_ganga:',
         'fr': ':bouton_bonne_affaire_en_japonais:',
         'ja': ':マル得:',
         'ko': ':얻을_득:',
         'pt': ':botão_japonês_de_“barganha”:',
         'it': ':ideogramma_giapponese_di_“occasione”:',
@@ -2354,15 +2354,15 @@
         'id': ':kastel_jepang:',
         'zh': ':日本城堡:'
     },
     '\U00003297\U0000FE0F': {  # ㊗️
         'en': ':Japanese_congratulations_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':congratulations:'],
+        'alias': [':congratulations:', ':japanese_congratulations_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_gratulation:',
         'es': ':ideograma_japonés_para_enhorabuena:',
         'fr': ':bouton_félicitations_en_japonais:',
         'ja': ':祝マーク:',
         'ko': ':원_안의_축하_표의문자:',
         'pt': ':botão_japonês_de_“parabéns”:',
@@ -2371,15 +2371,15 @@
         'id': ':tombol_jepang_selamat:',
         'zh': ':祝:'
     },
     '\U00003297': {  # ㊗
         'en': ':Japanese_congratulations_button:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':congratulations:'],
+        'alias': [':congratulations:', ':japanese_congratulations_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_gratulation:',
         'es': ':ideograma_japonés_para_enhorabuena:',
         'fr': ':bouton_félicitations_en_japonais:',
         'ja': ':祝マーク:',
         'ko': ':원_안의_축하_표의문자:',
         'pt': ':botão_japonês_de_“parabéns”:',
@@ -2388,15 +2388,15 @@
         'id': ':tombol_jepang_selamat:',
         'zh': ':祝:'
     },
     '\U0001F239': {  # 🈹
         'en': ':Japanese_discount_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u5272:'],
+        'alias': [':u5272:', ':japanese_discount_button:'],
         'de': ':schriftzeichen_für_rabatt:',
         'es': ':ideograma_japonés_para_descuento:',
         'fr': ':bouton_réduction_en_japonais:',
         'ja': ':割マーク:',
         'ko': ':나눌_할:',
         'pt': ':botão_japonês_de_“desconto”:',
         'it': ':ideogramma_giapponese_di_“sconto”:',
@@ -2404,15 +2404,15 @@
         'id': ':tombol_jepang_diskon:',
         'zh': ':割:'
     },
     '\U0001F38E': {  # 🎎
         'en': ':Japanese_dolls:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':dolls:'],
+        'alias': [':dolls:', ':japanese_dolls:'],
         'de': ':japanische_puppen:',
         'es': ':muñecas_japonesas:',
         'fr': ':poupées_japonaises:',
         'ja': ':ひな祭り:',
         'ko': ':일본_인형:',
         'pt': ':bonecas_japonesas:',
         'it': ':bambole_giapponesi:',
@@ -2420,15 +2420,15 @@
         'id': ':boneka_jepang:',
         'zh': ':日本人形:'
     },
     '\U0001F21A': {  # 🈚
         'en': ':Japanese_free_of_charge_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u7121:'],
+        'alias': [':u7121:', ':japanese_free_of_charge_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_gratis:',
         'es': ':ideograma_japonés_para_gratis:',
         'fr': ':bouton_gratuit_en_japonais:',
         'ja': ':無マーク:',
         'ko': ':없을_무:',
         'pt': ':botão_japonês_de_“gratuito”:',
@@ -2437,15 +2437,15 @@
         'id': ':tombol_jepang_gratis:',
         'zh': ':无:'
     },
     '\U0001F201': {  # 🈁
         'en': ':Japanese_here_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':koko:'],
+        'alias': [':koko:', ':japanese_here_button:'],
         'de': ':schriftzeichen_koko:',
         'es': ':ideograma_japonés_para_aquí:',
         'fr': ':bouton_ici_en_japonais:',
         'ja': ':ココのマーク:',
         'ko': ':일본어_여기_버튼:',
         'pt': ':botão_japonês_de_“aqui”:',
         'it': ':ideogramma_giapponese_per_“qui”:',
@@ -2453,15 +2453,15 @@
         'id': ':tombol_jepang_di_sini:',
         'zh': ':这里:'
     },
     '\U0001F237\U0000FE0F': {  # 🈷️
         'en': ':Japanese_monthly_amount_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u6708:'],
+        'alias': [':u6708:', ':japanese_monthly_amount_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_monatsbetrag:',
         'es': ':ideograma_japonés_para_cantidad_mensual:',
         'fr': ':bouton_montant_mensuel_en_japonais:',
         'ja': ':月マーク:',
         'ko': ':달_월:',
         'pt': ':botão_japonês_de_“quantidade_mensal”:',
@@ -2470,15 +2470,15 @@
         'id': ':tombol_jepang_jumlah_bulanan:',
         'zh': ':月:'
     },
     '\U0001F237': {  # 🈷
         'en': ':Japanese_monthly_amount_button:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':u6708:'],
+        'alias': [':u6708:', ':japanese_monthly_amount_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_monatsbetrag:',
         'es': ':ideograma_japonés_para_cantidad_mensual:',
         'fr': ':bouton_montant_mensuel_en_japonais:',
         'ja': ':月マーク:',
         'ko': ':달_월:',
         'pt': ':botão_japonês_de_“quantidade_mensal”:',
@@ -2487,15 +2487,15 @@
         'id': ':tombol_jepang_jumlah_bulanan:',
         'zh': ':月:'
     },
     '\U0001F235': {  # 🈵
         'en': ':Japanese_no_vacancy_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u6e80:'],
+        'alias': [':u6e80:', ':japanese_no_vacancy_button:'],
         'de': ':schriftzeichen_für_kein_zimmer_frei:',
         'es': ':ideograma_japonés_para_completo:',
         'fr': ':bouton_complet_en_japonais:',
         'ja': ':満マーク:',
         'ko': ':찰_만:',
         'pt': ':botão_japonês_de_“sem_vagas”:',
         'it': ':ideogramma_giapponese_di_“nessun_posto_libero”:',
@@ -2503,15 +2503,15 @@
         'id': ':tombol_jepang_tidak_ada_lowongan:',
         'zh': ':满:'
     },
     '\U0001F236': {  # 🈶
         'en': ':Japanese_not_free_of_charge_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u6709:'],
+        'alias': [':u6709:', ':japanese_not_free_of_charge_button:'],
         'de': ':schriftzeichen_für_nicht_gratis:',
         'es': ':ideograma_japonés_para_de_pago:',
         'fr': ':bouton_pas_gratuit_en_japonais:',
         'ja': ':有マーク:',
         'ko': ':있을_유:',
         'pt': ':botão_japonês_de_“não_gratuito”:',
         'it': ':ideogramma_giapponese_di_“a_pagamento”:',
@@ -2519,15 +2519,15 @@
         'id': ':tombol_jepang_tidak_gratis:',
         'zh': ':有:'
     },
     '\U0001F23A': {  # 🈺
         'en': ':Japanese_open_for_business_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u55b6:'],
+        'alias': [':u55b6:', ':japanese_open_for_business_button:'],
         'de': ':schriftzeichen_für_geöffnet:',
         'es': ':ideograma_japonés_para_abierto:',
         'fr': ':bouton_ouvert_pour_affaires_en_japonais:',
         'ja': ':営マーク:',
         'ko': ':벼슬_관:',
         'pt': ':botão_japonês_de_“aberto_para_negócios”:',
         'it': ':ideogramma_giapponese_di_“aperto_al_pubblico”:',
@@ -2535,15 +2535,15 @@
         'id': ':tombol_jepang_siap_berbisnis:',
         'zh': ':营:'
     },
     '\U0001F234': {  # 🈴
         'en': ':Japanese_passing_grade_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u5408:'],
+        'alias': [':u5408:', ':japanese_passing_grade_button:'],
         'de': ':schriftzeichen_für_note_zum_bestehen:',
         'es': ':ideograma_japonés_para_aprobado:',
         'fr': ':bouton_note_pour_réussir_en_japonais:',
         'ja': ':合マーク:',
         'ko': ':합할_합:',
         'pt': ':botão_japonês_de_“nota_mínima”:',
         'it': ':ideogramma_giapponese_di_“voto_di_sufficienza”:',
@@ -2551,15 +2551,15 @@
         'id': ':tombol_jepang_nilai_kelulusan:',
         'zh': ':合:'
     },
     '\U0001F3E3': {  # 🏣
         'en': ':Japanese_post_office:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':post_office:'],
+        'alias': [':post_office:', ':japanese_post_office:'],
         'de': ':japanisches_postgebäude:',
         'es': ':oficina_de_correos_japonesa:',
         'fr': ':bureau_de_poste_japonais:',
         'ja': ':郵便局:',
         'ko': ':일본_우체국:',
         'pt': ':correio_japonês:',
         'it': ':ufficio_postale_giapponese:',
@@ -2567,15 +2567,15 @@
         'id': ':kantor_pos_jepang:',
         'zh': ':日本邮局:'
     },
     '\U0001F232': {  # 🈲
         'en': ':Japanese_prohibited_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u7981:'],
+        'alias': [':u7981:', ':japanese_prohibited_button:'],
         'de': ':schriftzeichen_für_verbieten:',
         'es': ':ideograma_japonés_para_prohibido:',
         'fr': ':bouton_interdit_en_japonais:',
         'ja': ':禁マーク:',
         'ko': ':금할_금:',
         'pt': ':botão_japonês_de_“proibido”:',
         'it': ':ideogramma_giapponese_di_“proibito”:',
@@ -2583,15 +2583,15 @@
         'id': ':tombol_jepang_dilarang:',
         'zh': ':禁:'
     },
     '\U0001F22F': {  # 🈯
         'en': ':Japanese_reserved_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u6307:'],
+        'alias': [':u6307:', ':japanese_reserved_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_reserviert:',
         'es': ':ideograma_japonés_para_reservado:',
         'fr': ':bouton_réservé_en_japonais:',
         'ja': ':指マーク:',
         'ko': ':가리킬_지:',
         'pt': ':botão_japonês_de_“reservado”:',
@@ -2600,15 +2600,15 @@
         'id': ':tombol_jepang_sudah_dipesan:',
         'zh': ':指:'
     },
     '\U00003299\U0000FE0F': {  # ㊙️
         'en': ':Japanese_secret_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':secret:'],
+        'alias': [':secret:', ':japanese_secret_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_geheimnis:',
         'es': ':ideograma_japonés_para_secreto:',
         'fr': ':bouton_secret_en_japonais:',
         'ja': ':マル秘:',
         'ko': ':원_표시된_비밀_표의문자:',
         'pt': ':botão_japonês_de_“segredo”:',
@@ -2617,15 +2617,15 @@
         'id': ':tombol_jepang_rahasia:',
         'zh': ':秘:'
     },
     '\U00003299': {  # ㊙
         'en': ':Japanese_secret_button:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':secret:'],
+        'alias': [':secret:', ':japanese_secret_button:'],
         'variant': True,
         'de': ':schriftzeichen_für_geheimnis:',
         'es': ':ideograma_japonés_para_secreto:',
         'fr': ':bouton_secret_en_japonais:',
         'ja': ':マル秘:',
         'ko': ':원_표시된_비밀_표의문자:',
         'pt': ':botão_japonês_de_“segredo”:',
@@ -2634,15 +2634,15 @@
         'id': ':tombol_jepang_rahasia:',
         'zh': ':秘:'
     },
     '\U0001F202\U0000FE0F': {  # 🈂️
         'en': ':Japanese_service_charge_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':sa:'],
+        'alias': [':sa:', ':japanese_service_charge_button:'],
         'variant': True,
         'de': ':schriftzeichen_sa:',
         'es': ':ideograma_japonés_para_de_cortesía:',
         'fr': ':bouton_frais_de_service_en_japonais:',
         'ja': ':サのマーク:',
         'ko': ':일본어_봉사료_버튼:',
         'pt': ':botão_japonês_de_“taxa_de_serviço”:',
@@ -2651,15 +2651,15 @@
         'id': ':tombol_jepang_biaya_layanan:',
         'zh': ':服务费:'
     },
     '\U0001F202': {  # 🈂
         'en': ':Japanese_service_charge_button:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':sa:'],
+        'alias': [':sa:', ':japanese_service_charge_button:'],
         'variant': True,
         'de': ':schriftzeichen_sa:',
         'es': ':ideograma_japonés_para_de_cortesía:',
         'fr': ':bouton_frais_de_service_en_japonais:',
         'ja': ':サのマーク:',
         'ko': ':일본어_봉사료_버튼:',
         'pt': ':botão_japonês_de_“taxa_de_serviço”:',
@@ -2668,15 +2668,15 @@
         'id': ':tombol_jepang_biaya_layanan:',
         'zh': ':服务:'
     },
     '\U0001F530': {  # 🔰
         'en': ':Japanese_symbol_for_beginner:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':beginner:'],
+        'alias': [':beginner:', ':japanese_symbol_for_beginner:'],
         'de': ':japanisches_anfänger-zeichen:',
         'es': ':símbolo_japonés_para_principiante:',
         'fr': ':symbole_japonais_de_débutant:',
         'ja': ':初心者マーク:',
         'ko': ':노란색_초록색_이파리_모양:',
         'pt': ':símbolo_japonês_de_principiante:',
         'it': ':ideogramma_giapponese_di_“principiante”:',
@@ -2684,15 +2684,15 @@
         'id': ':simbol_jepang_untuk_pemula:',
         'zh': ':日本新手驾驶标志:'
     },
     '\U0001F233': {  # 🈳
         'en': ':Japanese_vacancy_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':u7a7a:'],
+        'alias': [':u7a7a:', ':japanese_vacancy_button:'],
         'de': ':schriftzeichen_für_zimmer_frei:',
         'es': ':ideograma_japonés_para_vacante:',
         'fr': ':bouton_chambres_disponibles_en_japonais:',
         'ja': ':空マーク:',
         'ko': ':빌_공:',
         'pt': ':botão_japonês_de_“vago”:',
         'it': ':ideogramma_giapponese_di_“posto_libero”:',
@@ -3449,15 +3449,15 @@
         'id': ':bendera_myanmar_(burma):',
         'zh': ':缅甸:'
     },
     '\U0001F195': {  # 🆕
         'en': ':NEW_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':new:'],
+        'alias': [':new:', ':new_button:'],
         'de': ':wort_new_in_blauem_quadrat:',
         'es': ':botón_new:',
         'fr': ':bouton_nouveau:',
         'ja': ':newマーク:',
         'ko': ':뉴:',
         'pt': ':botão_new:',
         'it': ':pulsante_new:',
@@ -3465,15 +3465,15 @@
         'id': ':tombol_new:',
         'zh': ':new按钮:'
     },
     '\U0001F196': {  # 🆖
         'en': ':NG_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':ng:'],
+        'alias': [':ng:', ':ng_button:'],
         'de': ':großbuchstaben_ng_in_blauem_quadrat:',
         'es': ':botón_ng:',
         'fr': ':bouton_pas_bien:',
         'ja': ':ngマーク:',
         'ko': ':엔지:',
         'pt': ':botão_ng:',
         'it': ':pulsante_ng:',
@@ -3721,15 +3721,15 @@
         'id': ':bendera_norwegia:',
         'zh': ':挪威:'
     },
     '\U0001F197': {  # 🆗
         'en': ':OK_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':ok:'],
+        'alias': [':ok:', ':ok_button:'],
         'de': ':großbuchstaben_ok_in_blauem_quadrat:',
         'es': ':botón_ok:',
         'fr': ':bouton_ok:',
         'ja': ':okマーク:',
         'ko': ':오케이:',
         'pt': ':botão_ok:',
         'it': ':pulsante_ok:',
@@ -3828,15 +3828,15 @@
         'id': ':oke_warna_kulit_sedang:',
         'zh': ':OK_中等肤色:'
     },
     '\U0001F51B': {  # 🔛
         'en': ':ON!_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':on:'],
+        'alias': [':on:', ':on_arrow:', ':on!_arrow:'],
         'de': ':on!-pfeil:',
         'es': ':flecha_on!:',
         'fr': ':flèche_activé:',
         'ja': ':on矢印:',
         'ko': ':켜짐:',
         'pt': ':seta_on!:',
         'it': ':freccia_on:',
@@ -3844,15 +3844,15 @@
         'id': ':tanda_panah_on!:',
         'zh': ':ON箭头:'
     },
     '\U0001F17E\U0000FE0F': {  # 🅾️
         'en': ':O_button_(blood_type):',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':o2:'],
+        'alias': [':o2:', ':o_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_o_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_tipo_o:',
         'fr': ':groupe_sanguin_o:',
         'ja': ':血液型o型:',
         'ko': ':오형:',
         'pt': ':botão_o_(tipo_sanguíneo):',
@@ -3861,15 +3861,15 @@
         'id': ':tombol_o_(golongan_darah):',
         'zh': ':O型血:'
     },
     '\U0001F17E': {  # 🅾
         'en': ':O_button_(blood_type):',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':o2:'],
+        'alias': [':o2:', ':o_button_blood_type:'],
         'variant': True,
         'de': ':großbuchstabe_o_in_rotem_quadrat:',
         'es': ':grupo_sanguíneo_tipo_o:',
         'fr': ':groupe_sanguin_o:',
         'ja': ':血液型o型:',
         'ko': ':오형:',
         'pt': ':botão_o_(tipo_sanguíneo):',
@@ -3910,15 +3910,15 @@
         'id': ':ophiuchus:',
         'zh': ':蛇夫座:'
     },
     '\U0001F17F\U0000FE0F': {  # 🅿️
         'en': ':P_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':parking:'],
+        'alias': [':parking:', ':p_button:'],
         'variant': True,
         'de': ':großbuchstabe_p_in_blauem_quadrat:',
         'es': ':aparcamiento:',
         'fr': ':bouton_p:',
         'ja': ':pマーク:',
         'ko': ':주차_표시:',
         'pt': ':botão_p:',
@@ -3927,15 +3927,15 @@
         'id': ':tombol_p:',
         'zh': ':停车按钮:'
     },
     '\U0001F17F': {  # 🅿
         'en': ':P_button:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':parking:'],
+        'alias': [':parking:', ':p_button:'],
         'variant': True,
         'de': ':großbuchstabe_p_in_blauem_quadrat:',
         'es': ':aparcamiento:',
         'fr': ':bouton_p:',
         'ja': ':pマーク:',
         'ko': ':주차_표시:',
         'pt': ':botão_p:',
@@ -4233,15 +4233,15 @@
         'id': ':bendera_réunion:',
         'zh': ':留尼汪:'
     },
     '\U0001F51C': {  # 🔜
         'en': ':SOON_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':soon:'],
+        'alias': [':soon:', ':soon_arrow:'],
         'de': ':soon-pfeil:',
         'es': ':flecha_soon:',
         'fr': ':flèche_bientôt:',
         'ja': ':soon矢印:',
         'ko': ':곧:',
         'pt': ':seta_soon:',
         'it': ':freccia_soon:',
@@ -4249,15 +4249,15 @@
         'id': ':tanda_panah_soon:',
         'zh': ':SOON箭头:'
     },
     '\U0001F198': {  # 🆘
         'en': ':SOS_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':sos:'],
+        'alias': [':sos:', ':sos_button:'],
         'de': ':sos-zeichen:',
         'es': ':símbolo_de_socorro:',
         'fr': ':bouton_sos:',
         'ja': ':sosマーク:',
         'ko': ':에스오에스:',
         'pt': ':botão_sos:',
         'it': ':pulsante_sos:',
@@ -4314,15 +4314,15 @@
         'id': ':bendera_san_marino:',
         'zh': ':圣马力诺:'
     },
     '\U0001F385': {  # 🎅
         'en': ':Santa_Claus:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':santa:'],
+        'alias': [':santa:', ':santa_claus:'],
         'de': ':weihnachtsmann:',
         'es': ':papá_noel:',
         'fr': ':père_noël:',
         'ja': ':サンタ:',
         'ko': ':산타클로스:',
         'pt': ':papai_noel:',
         'it': ':babbo_natale:',
@@ -4421,15 +4421,15 @@
         'id': ':bendera_arab_saudi:',
         'zh': ':沙特阿拉伯:'
     },
     '\U0000264F': {  # ♏
         'en': ':Scorpio:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':scorpius:'],
+        'alias': [':scorpius:', ':scorpio:'],
         'variant': True,
         'de': ':skorpion_(sternzeichen):',
         'es': ':escorpio:',
         'fr': ':scorpion_zodiaque:',
         'ja': ':さそり座:',
         'ko': ':전갈자리:',
         'pt': ':signo_de_escorpião:',
@@ -4950,15 +4950,15 @@
         'id': ':bendera_sao_tome_dan_principe:',
         'zh': ':圣多美和普林西比:'
     },
     '\U0001F996': {  # 🦖
         'en': ':T-Rex:',
         'status': fully_qualified,
         'E': 5,
-        'alias': [':t-rex:'],
+        'alias': [':t-rex:', ':t_rex:'],
         'de': ':t-rex:',
         'es': ':t-rex:',
         'fr': ':t-rex:',
         'ja': ':ティラノサウルス:',
         'ko': ':티라노사우루스:',
         'pt': ':tiranossauro_rex:',
         'it': ':t-rex:',
@@ -4966,15 +4966,15 @@
         'id': ':t-rex:',
         'zh': ':霸王龙:'
     },
     '\U0001F51D': {  # 🔝
         'en': ':TOP_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':top:'],
+        'alias': [':top:', ':top_arrow:'],
         'de': ':top-pfeil:',
         'es': ':flecha_top:',
         'fr': ':flèche_en_haut:',
         'ja': ':top矢印:',
         'ko': ':위로_화살표:',
         'pt': ':seta_top:',
         'it': ':freccia_top:',
@@ -5287,15 +5287,15 @@
         'id': ':bendera_kepulauan_virgin_amerika_serikat:',
         'zh': ':美属维尔京群岛:'
     },
     '\U0001F199': {  # 🆙
         'en': ':UP!_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':up:'],
+        'alias': [':up:', ':up_button:'],
         'de': ':schriftzug_up!_im_blauen_quadrat:',
         'es': ':botón_up!:',
         'fr': ':bouton_vers_le_haut:',
         'ja': ':upマーク:',
         'ko': ':위로_버튼:',
         'pt': ':botão_up!:',
         'it': ':pulsante_up!:',
@@ -5431,15 +5431,15 @@
         'id': ':bendera_uzbekistan:',
         'zh': ':乌兹别克斯坦:'
     },
     '\U0001F19A': {  # 🆚
         'en': ':VS_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':vs:'],
+        'alias': [':vs:', ':vs_button:'],
         'de': ':schriftzug_vs_in_orangem_quadrat:',
         'es': ':botón_vs:',
         'fr': ':bouton_vs:',
         'ja': ':vsマーク:',
         'ko': ':대:',
         'pt': ':botão_vs:',
         'it': ':pulsante_vs:',
@@ -9934,15 +9934,15 @@
         'id': ':film:',
         'zh': ':电影院:'
     },
     '\U000024C2\U0000FE0F': {  # Ⓜ️
         'en': ':circled_M:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':m:'],
+        'alias': [':m:', ':circled_m:'],
         'variant': True,
         'de': ':buchstabe_m_in_kreis:',
         'es': ':m_en_círculo:',
         'fr': ':m_encerclé:',
         'ja': ':丸いmマーク:',
         'ko': ':원글자_엠:',
         'pt': ':círculo_com_a_letra_m:',
@@ -9951,15 +9951,15 @@
         'id': ':huruf_m_dalam_lingkaran:',
         'zh': ':圆圈包围的M:'
     },
     '\U000024C2': {  # Ⓜ
         'en': ':circled_M:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':m:'],
+        'alias': [':m:', ':circled_m:'],
         'variant': True,
         'de': ':buchstabe_m_in_kreis:',
         'es': ':m_en_círculo:',
         'fr': ':m_encerclé:',
         'ja': ':丸いmマーク:',
         'ko': ':원글자_엠:',
         'pt': ':círculo_com_a_letra_m:',
@@ -11245,26 +11245,36 @@
     '\U0001F491\U0001F3FF': {  # 💑🏿
         'en': ':couple_with_heart_dark_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_dunkle_hautfarbe:',
         'es': ':pareja_enamorada_tono_de_piel_oscuro:',
         'fr': ':couple_avec_cœur__peau_foncée:',
+        'ja': ':カップルとハート_濃い肌色:',
+        'ko': ':연인_검은색_피부:',
         'pt': ':casal_apaixonado_pele_escura:',
-        'it': ':coppia_con_cuore_carnagione_scura:'
+        'it': ':coppia_con_cuore_carnagione_scura:',
+        'fa': ':زوج_عاشق_پوست_آبنوسی:',
+        'id': ':pasangan_dengan_hati_warna_kulit_gelap:',
+        'zh': ':情侣_较深肤色:'
     },
     '\U0001F491\U0001F3FB': {  # 💑🏻
         'en': ':couple_with_heart_light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_helle_hautfarbe:',
         'es': ':pareja_enamorada_tono_de_piel_claro:',
         'fr': ':couple_avec_cœur__peau_claire:',
+        'ja': ':カップルとハート_薄い肌色:',
+        'ko': ':연인_하얀_피부:',
         'pt': ':casal_apaixonado_pele_clara:',
-        'it': ':coppia_con_cuore_carnagione_chiara:'
+        'it': ':coppia_con_cuore_carnagione_chiara:',
+        'fa': ':زوج_عاشق_پوست_سفید:',
+        'id': ':pasangan_dengan_hati_warna_kulit_cerah:',
+        'zh': ':情侣_较浅肤色:'
     },
     '\U0001F468\U0000200D\U00002764\U0000FE0F\U0000200D\U0001F468': {  # 👨‍❤️‍👨
         'en': ':couple_with_heart_man_man:',
         'status': fully_qualified,
         'E': 2,
         'de': ':liebespaar_mann,_mann:',
         'es': ':pareja_enamorada_hombre_y_hombre:',
@@ -11785,36 +11795,51 @@
     '\U0001F491\U0001F3FE': {  # 💑🏾
         'en': ':couple_with_heart_medium-dark_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_mitteldunkle_hautfarbe:',
         'es': ':pareja_enamorada_tono_de_piel_oscuro_medio:',
         'fr': ':couple_avec_cœur__peau_mate:',
+        'ja': ':カップルとハート_やや濃い肌色:',
+        'ko': ':연인_진한_갈색_피부:',
         'pt': ':casal_apaixonado_pele_morena_escura:',
-        'it': ':coppia_con_cuore_carnagione_abbastanza_scura:'
+        'it': ':coppia_con_cuore_carnagione_abbastanza_scura:',
+        'fa': ':زوج_عاشق_پوست_گندمی:',
+        'id': ':pasangan_dengan_hati_warna_kulit_gelap-sedang:',
+        'zh': ':情侣_中等深肤色:'
     },
     '\U0001F491\U0001F3FC': {  # 💑🏼
         'en': ':couple_with_heart_medium-light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_mittelhelle_hautfarbe:',
         'es': ':pareja_enamorada_tono_de_piel_claro_medio:',
         'fr': ':couple_avec_cœur__peau_moyennement_claire:',
+        'ja': ':カップルとハート_やや薄い肌色:',
+        'ko': ':연인_연한_갈색_피부:',
         'pt': ':casal_apaixonado_pele_morena_clara:',
-        'it': ':coppia_con_cuore_carnagione_abbastanza_chiara:'
+        'it': ':coppia_con_cuore_carnagione_abbastanza_chiara:',
+        'fa': ':زوج_عاشق_پوست_روشن:',
+        'id': ':pasangan_dengan_hati_warna_kulit_cerah-sedang:',
+        'zh': ':情侣_中等浅肤色:'
     },
     '\U0001F491\U0001F3FD': {  # 💑🏽
         'en': ':couple_with_heart_medium_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_mittlere_hautfarbe:',
         'es': ':pareja_enamorada_tono_de_piel_medio:',
         'fr': ':couple_avec_cœur__peau_légèrement_mate:',
+        'ja': ':カップルとハート_中間の肌色:',
+        'ko': ':연인_갈색_피부:',
         'pt': ':casal_apaixonado_pele_morena:',
-        'it': ':coppia_con_cuore_carnagione_olivastra:'
+        'it': ':coppia_con_cuore_carnagione_olivastra:',
+        'fa': ':زوج_عاشق_پوست_طلایی:',
+        'id': ':pasangan_dengan_hati_warna_kulit_sedang:',
+        'zh': ':情侣_中等肤色:'
     },
     '\U0001F9D1\U0001F3FF\U0000200D\U00002764\U0000FE0F\U0000200D\U0001F9D1\U0001F3FB': {  # 🧑🏿‍❤️‍🧑🏻
         'en': ':couple_with_heart_person_person_dark_skin_tone_light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':liebespaar_erwachsener_erwachsener_dunkle_hautfarbe,helle_hautfarbe:',
         'es': ':pareja_enamorada_persona_adulta_persona_adulta_tono_de_piel_oscuro_tono_de_piel_claro:',
@@ -14996,15 +15021,15 @@
         'id': ':wajah_dengan_garis_titik-titik:',
         'zh': ':虚线脸:'
     },
     '\U0001F52F': {  # 🔯
         'en': ':dotted_six-pointed_star:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':six_pointed_star:'],
+        'alias': [':six_pointed_star:', ':dotted_six_pointed_star:'],
         'de': ':hexagramm_mit_punkt:',
         'es': ':estrella_de_seis_puntas:',
         'fr': ':étoile_à_6_branches:',
         'ja': ':六芒星:',
         'ko': ':육각_별:',
         'pt': ':estrela_de_seis_pontas:',
         'it': ':stella_a_sei_punte:',
@@ -15111,15 +15136,15 @@
         'id': ':merpati:',
         'zh': ':鸽:'
     },
     '\U00002199\U0000FE0F': {  # ↙️
         'en': ':down-left_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':arrow_lower_left:'],
+        'alias': [':arrow_lower_left:', ':down_left_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_links_unten:',
         'es': ':flecha_hacia_la_esquina_inferior_izquierda:',
         'fr': ':flèche_bas_gauche:',
         'ja': ':左下矢印:',
         'ko': ':좌하향_화살표:',
         'pt': ':seta_para_baixo_e_para_a_esquerda:',
@@ -15128,15 +15153,15 @@
         'id': ':tanda_panah_kiri_bawah:',
         'zh': ':左下箭头:'
     },
     '\U00002199': {  # ↙
         'en': ':down-left_arrow:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':arrow_lower_left:'],
+        'alias': [':arrow_lower_left:', ':down_left_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_links_unten:',
         'es': ':flecha_hacia_la_esquina_inferior_izquierda:',
         'fr': ':flèche_bas_gauche:',
         'ja': ':左下矢印:',
         'ko': ':좌하향_화살표:',
         'pt': ':seta_para_baixo_e_para_a_esquerda:',
@@ -15145,15 +15170,15 @@
         'id': ':tanda_panah_kiri_bawah:',
         'zh': ':左下箭头:'
     },
     '\U00002198\U0000FE0F': {  # ↘️
         'en': ':down-right_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':arrow_lower_right:'],
+        'alias': [':arrow_lower_right:', ':down_right_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_rechts_unten:',
         'es': ':flecha_hacia_la_esquina_inferior_derecha:',
         'fr': ':flèche_bas_droite:',
         'ja': ':右下矢印:',
         'ko': ':우하향_화살표:',
         'pt': ':seta_para_baixo_e_para_a_direita:',
@@ -15162,15 +15187,15 @@
         'id': ':tanda_panah_kanan_bawah:',
         'zh': ':右下箭头:'
     },
     '\U00002198': {  # ↘
         'en': ':down-right_arrow:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':arrow_lower_right:'],
+        'alias': [':arrow_lower_right:', ':down_right_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_rechts_unten:',
         'es': ':flecha_hacia_la_esquina_inferior_derecha:',
         'fr': ':flèche_bas_droite:',
         'ja': ':右下矢印:',
         'ko': ':우하향_화살표:',
         'pt': ':seta_para_baixo_e_para_a_direita:',
@@ -15395,15 +15420,15 @@
         'id': ':dvd:',
         'zh': ':DVD:'
     },
     '\U0001F4E7': {  # 📧
         'en': ':e-mail:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':email:', ':e__mail:'],
+        'alias': [':email:', ':e__mail:', ':e_mail:'],
         'de': ':e-mail:',
         'es': ':correo_electrónico:',
         'fr': ':e-mail:',
         'ja': ':eメール:',
         'ko': ':이메일:',
         'pt': ':e-mail:',
         'it': ':e-mail:',
@@ -15654,15 +15679,15 @@
         'id': ':terung:',
         'zh': ':茄子:'
     },
     '\U00002734\U0000FE0F': {  # ✴️
         'en': ':eight-pointed_star:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':eight_pointed_black_star:'],
+        'alias': [':eight_pointed_black_star:', ':eight_pointed_star:'],
         'variant': True,
         'de': ':stern_mit_acht_zacken:',
         'es': ':estrella_de_ocho_puntas:',
         'fr': ':étoile_huit_branches:',
         'ja': ':八角星:',
         'ko': ':팔각_별:',
         'pt': ':estrela_de_oito_pontas:',
@@ -15671,15 +15696,15 @@
         'id': ':bintang_berujung_delapan:',
         'zh': ':八角星:'
     },
     '\U00002734': {  # ✴
         'en': ':eight-pointed_star:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':eight_pointed_black_star:'],
+        'alias': [':eight_pointed_black_star:', ':eight_pointed_star:'],
         'variant': True,
         'de': ':achtstrahliger_stern:',
         'es': ':estrella_de_ocho_puntas:',
         'fr': ':étoile_huit_branches:',
         'ja': ':八角星:',
         'ko': ':팔각_별:',
         'pt': ':estrela_de_oito_pontas:',
@@ -15722,15 +15747,15 @@
         'id': ':bintang_berujung_lancip_delapan:',
         'zh': ':八轮辐星号:'
     },
     '\U0001F563': {  # 🕣
         'en': ':eight-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock830:'],
+        'alias': [':clock830:', ':eight_thirty:'],
         'variant': True,
         'de': ':8.30_uhr:',
         'es': ':ocho_y_media:',
         'fr': ':huit_heures_et_demie:',
         'ja': ':8時半:',
         'ko': ':여덟_시_반:',
         'pt': ':oito_e_meia:',
@@ -15739,15 +15764,15 @@
         'id': ':jam_setengah_sembilan:',
         'zh': ':八点半:'
     },
     '\U0001F557': {  # 🕗
         'en': ':eight_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock8:'],
+        'alias': [':clock8:', ':eight_oclock:'],
         'variant': True,
         'de': ':8.00_uhr:',
         'es': ':8_en_punto:',
         'fr': ':huit_heures:',
         'ja': ':8時:',
         'ko': ':여덟_시:',
         'pt': ':8_horas:',
@@ -15835,15 +15860,15 @@
         'id': ':elevator:',
         'zh': ':电梯:'
     },
     '\U0001F566': {  # 🕦
         'en': ':eleven-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock1130:'],
+        'alias': [':clock1130:', ':eleven_thirty:'],
         'variant': True,
         'de': ':11.30_uhr:',
         'es': ':once_y_media:',
         'fr': ':onze_heures_et_demie:',
         'ja': ':11時半:',
         'ko': ':열한_시_반:',
         'pt': ':onze_e_meia:',
@@ -15852,15 +15877,15 @@
         'id': ':jam_setengah_dua_belas:',
         'zh': ':十一点半:'
     },
     '\U0001F55A': {  # 🕚
         'en': ':eleven_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock11:'],
+        'alias': [':clock11:', ':eleven_oclock:'],
         'variant': True,
         'de': ':11.00_uhr:',
         'es': ':11_en_punto:',
         'fr': ':onze_heures:',
         'ja': ':11時:',
         'ko': ':열한_시:',
         'pt': ':11_horas:',
@@ -16382,15 +16407,15 @@
         'id': ':wajah_muntah:',
         'zh': ':呕吐:'
     },
     '\U0001F635': {  # 😵
         'en': ':face_with_crossed-out_eyes:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':dizzy_face:'],
+        'alias': [':dizzy_face:', ':face_with_crossed_out_eyes:', ':knocked_out_face:'],
         'de': ':benommenes_gesicht:',
         'es': ':cara_mareada:',
         'fr': ':visage_étourdi:',
         'ja': ':めまい:',
         'ko': ':어지러운_얼굴:',
         'pt': ':rosto_atordoado:',
         'it': ':faccina_frastornata:',
@@ -17372,15 +17397,15 @@
         'id': ':petani_warna_kulit_sedang:',
         'zh': ':农民_中等肤色:'
     },
     '\U000023E9': {  # ⏩
         'en': ':fast-forward_button:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':fast_forward:'],
+        'alias': [':fast_forward:', ':fast_forward_button:'],
         'variant': True,
         'de': ':doppelpfeile_nach_rechts:',
         'es': ':avance_rápido:',
         'fr': ':bouton_avance_rapide:',
         'ja': ':早送りボタン:',
         'ko': ':빨리_감기:',
         'pt': ':botão_avançar:',
@@ -17937,15 +17962,15 @@
         'id': ':tongkat_pancing:',
         'zh': ':钓鱼竿:'
     },
     '\U0001F560': {  # 🕠
         'en': ':five-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock530:'],
+        'alias': [':clock530:', ':five_thirty:'],
         'variant': True,
         'de': ':5.30_uhr:',
         'es': ':cinco_y_media:',
         'fr': ':cinq_heures_et_demie:',
         'ja': ':5時半:',
         'ko': ':다섯_시_반:',
         'pt': ':cinco_e_meia:',
@@ -17954,15 +17979,15 @@
         'id': ':jam_setengah_enam:',
         'zh': ':五点半:'
     },
     '\U0001F554': {  # 🕔
         'en': ':five_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock5:'],
+        'alias': [':clock5:', ':five_oclock:'],
         'variant': True,
         'de': ':5.00_uhr:',
         'es': ':5_en_punto:',
         'fr': ':cinq_heures:',
         'ja': ':5時:',
         'ko': ':다섯_시:',
         'pt': ':5_horas:',
@@ -18666,15 +18691,15 @@
         'id': ':pena_tinta:',
         'zh': ':钢笔:'
     },
     '\U0001F55F': {  # 🕟
         'en': ':four-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock430:'],
+        'alias': [':clock430:', ':four_thirty:'],
         'variant': True,
         'de': ':4.30_uhr:',
         'es': ':cuatro_y_media:',
         'fr': ':quatre_heures_et_demie:',
         'ja': ':4時半:',
         'ko': ':네_시_반:',
         'pt': ':quatro_e_meia:',
@@ -18698,15 +18723,15 @@
         'id': ':empat_daun_semanggi:',
         'zh': ':四叶草:'
     },
     '\U0001F553': {  # 🕓
         'en': ':four_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock4:'],
+        'alias': [':clock4:', ':four_oclock:'],
         'variant': True,
         'de': ':4.00_uhr:',
         'es': ':4_en_punto:',
         'fr': ':quatre_heures:',
         'ja': ':4時:',
         'ko': ':네_시:',
         'pt': ':4_horas:',
@@ -18811,15 +18836,15 @@
         'id': ':katak:',
         'zh': ':青蛙:'
     },
     '\U0001F425': {  # 🐥
         'en': ':front-facing_baby_chick:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':hatched_chick:'],
+        'alias': [':hatched_chick:', ':front_facing_baby_chick:'],
         'de': ':küken_von_vorne:',
         'es': ':pollito_de_frente:',
         'fr': ':poussin_de_face:',
         'ja': ':前を向いているひよこ:',
         'ko': ':정면을_향해_날개를_편_병아리:',
         'pt': ':pintinho_de_frente:',
         'it': ':pulcino_visto_di_fronte:',
@@ -19219,15 +19244,15 @@
         'id': ':kacamata:',
         'zh': ':眼镜:'
     },
     '\U0001F30E': {  # 🌎
         'en': ':globe_showing_Americas:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':earth_americas:'],
+        'alias': [':earth_americas:', ':globe_showing_americas:'],
         'variant': True,
         'de': ':globus_mit_amerika:',
         'es': ':globo_terráqueo_mostrando_américa:',
         'fr': ':globe_tourné_sur_les_amériques:',
         'ja': ':地球(アメリカ大陸):',
         'ko': ':미대륙이_보이는_지구:',
         'pt': ':globo_mostrando_as_américas:',
@@ -19236,15 +19261,15 @@
         'id': ':bola_dunia_amerika:',
         'zh': ':地球上的美洲:'
     },
     '\U0001F30F': {  # 🌏
         'en': ':globe_showing_Asia-Australia:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':earth_asia:'],
+        'alias': [':earth_asia:', ':globe_showing_asia_australia:'],
         'variant': True,
         'de': ':globus_mit_asien_und_australien:',
         'es': ':globo_terráqueo_mostrando_asia_y_australia:',
         'fr': ':globe_tourné_sur_l’asie_et_l’australie:',
         'ja': ':地球(アジアとオーストラリア):',
         'ko': ':아시아와_호주가_보이는_지구:',
         'pt': ':globo_mostrando_ásia_e_oceania:',
@@ -19253,15 +19278,15 @@
         'id': ':bola_dunia_asia-australia:',
         'zh': ':地球上的亚洲澳洲:'
     },
     '\U0001F30D': {  # 🌍
         'en': ':globe_showing_Europe-Africa:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':earth_africa:'],
+        'alias': [':earth_africa:', ':globe_showing_europe_africa:'],
         'variant': True,
         'de': ':globus_mit_europa_und_afrika:',
         'es': ':globo_terráqueo_mostrando_europa_y_áfrica:',
         'fr': ':globe_tourné_sur_l’afrique_et_l’europe:',
         'ja': ':地球(ヨーロッパとアフリカ):',
         'ko': ':유럽과_아프리카가_보이는_지구:',
         'pt': ':globo_mostrando_europa_e_áfrica:',
@@ -19392,14 +19417,15 @@
         'id': ':angsa_leher_pendek:',
         'zh': ':鹅:'
     },
     '\U0001F98D': {  # 🦍
         'en': ':gorilla:',
         'status': fully_qualified,
         'E': 3,
+        'alias': [':harambe:'],
         'de': ':gorilla:',
         'es': ':gorila:',
         'fr': ':gorille:',
         'ja': ':ゴリラ:',
         'ko': ':고릴라:',
         'pt': ':gorila:',
         'it': ':gorilla:',
@@ -20070,35 +20096,85 @@
         'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع:',
         'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang:',
         'zh': ':食指与拇指交叉的手:'
     },
     '\U0001FAF0\U0001F3FF': {  # 🫰🏿
         'en': ':hand_with_index_finger_and_thumb_crossed_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_gekreuztem_zeigefinger_und_daumen_dunkle_hautfarbe:',
+        'es': ':mano_con_dedo_índice_y_pulgar_cruzados_tono_de_piel_oscuro:',
+        'fr': ':main_avec_index_et_pouce_croisés__peau_foncée:',
+        'ja': ':親指と人差し指をクロス_濃い肌色:',
+        'ko': ':엄지와_중지를_교차한_손_검은색_피부:',
+        'pt': ':mão_com_dedo_indicador_e_polegar_cruzados_pele_escura:',
+        'it': ':mano_con_indice_e_pollice_incrociati_carnagione_scura:',
+        'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع_پوست_آبنوسی:',
+        'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang_warna_kulit_gelap:',
+        'zh': ':食指与拇指交叉的手_较深肤色:'
     },
     '\U0001FAF0\U0001F3FB': {  # 🫰🏻
         'en': ':hand_with_index_finger_and_thumb_crossed_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_gekreuztem_zeigefinger_und_daumen_helle_hautfarbe:',
+        'es': ':mano_con_dedo_índice_y_pulgar_cruzados_tono_de_piel_claro:',
+        'fr': ':main_avec_index_et_pouce_croisés__peau_claire:',
+        'ja': ':親指と人差し指をクロス_薄い肌色:',
+        'ko': ':엄지와_중지를_교차한_손_하얀_피부:',
+        'pt': ':mão_com_dedo_indicador_e_polegar_cruzados_pele_clara:',
+        'it': ':mano_con_indice_e_pollice_incrociati_carnagione_chiara:',
+        'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع_پوست_سفید:',
+        'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang_warna_kulit_cerah:',
+        'zh': ':食指与拇指交叉的手_较浅肤色:'
     },
     '\U0001FAF0\U0001F3FE': {  # 🫰🏾
         'en': ':hand_with_index_finger_and_thumb_crossed_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_gekreuztem_zeigefinger_und_daumen_mitteldunkle_hautfarbe:',
+        'es': ':mano_con_dedo_índice_y_pulgar_cruzados_tono_de_piel_oscuro_medio:',
+        'fr': ':main_avec_index_et_pouce_croisés__peau_mate:',
+        'ja': ':親指と人差し指をクロス_やや濃い肌色:',
+        'ko': ':엄지와_중지를_교차한_손_진한_갈색_피부:',
+        'pt': ':mão_com_dedo_indicador_e_polegar_cruzados_pele_morena_escura:',
+        'it': ':mano_con_indice_e_pollice_incrociati_carnagione_abbastanza_scura:',
+        'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع_پوست_گندمی:',
+        'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang_warna_kulit_gelap-sedang:',
+        'zh': ':食指与拇指交叉的手_中等深肤色:'
     },
     '\U0001FAF0\U0001F3FC': {  # 🫰🏼
         'en': ':hand_with_index_finger_and_thumb_crossed_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_gekreuztem_zeigefinger_und_daumen_mittelhelle_hautfarbe:',
+        'es': ':mano_con_dedo_índice_y_pulgar_cruzados_tono_de_piel_claro_medio:',
+        'fr': ':main_avec_index_et_pouce_croisés__peau_moyennement_claire:',
+        'ja': ':親指と人差し指をクロス_やや薄い肌色:',
+        'ko': ':엄지와_중지를_교차한_손_연한_갈색_피부:',
+        'pt': ':mão_com_dedo_indicador_e_polegar_cruzados_pele_morena_clara:',
+        'it': ':mano_con_indice_e_pollice_incrociati_carnagione_abbastanza_chiara:',
+        'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع_پوست_روشن:',
+        'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang_warna_kulit_cerah-sedang:',
+        'zh': ':食指与拇指交叉的手_中等浅肤色:'
     },
     '\U0001FAF0\U0001F3FD': {  # 🫰🏽
         'en': ':hand_with_index_finger_and_thumb_crossed_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_gekreuztem_zeigefinger_und_daumen_mittlere_hautfarbe:',
+        'es': ':mano_con_dedo_índice_y_pulgar_cruzados_tono_de_piel_medio:',
+        'fr': ':main_avec_index_et_pouce_croisés__peau_légèrement_mate:',
+        'ja': ':親指と人差し指をクロス_中間の肌色:',
+        'ko': ':엄지와_중지를_교차한_손_갈색_피부:',
+        'pt': ':mão_com_dedo_indicador_e_polegar_cruzados_pele_morena:',
+        'it': ':mano_con_indice_e_pollice_incrociati_carnagione_olivastra:',
+        'fa': ':دست_با_انگشت_اشاره_و_شست_متقاطع_پوست_طلایی:',
+        'id': ':tangan_dengan_jari_telunjuk_dan_ibu_jari_menyilang_warna_kulit_sedang:',
+        'zh': ':食指与拇指交叉的手_中等肤色:'
     },
     '\U0001F45C': {  # 👜
         'en': ':handbag:',
         'status': fully_qualified,
         'E': 0.6,
         'de': ':handtasche:',
         'es': ':bolso:',
@@ -20125,135 +20201,385 @@
         'fa': ':دست_دادن:',
         'id': ':jabat_tangan:',
         'zh': ':握手:'
     },
     '\U0001F91D\U0001F3FF': {  # 🤝🏿
         'en': ':handshake_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_dunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro:',
+        'fr': ':poignée_de_main__peau_foncée:',
+        'ja': ':握手_濃い肌色:',
+        'ko': ':악수_검은색_피부:',
+        'pt': ':aperto_de_mãos_pele_escura:',
+        'it': ':stretta_di_mano_carnagione_scura:',
+        'fa': ':دست_دادن_پوست_آبنوسی:',
+        'id': ':jabat_tangan_warna_kulit_gelap:',
+        'zh': ':握手_较深肤色:'
     },
     '\U0001FAF1\U0001F3FF\U0000200D\U0001FAF2\U0001F3FB': {  # 🫱🏿‍🫲🏻
         'en': ':handshake_dark_skin_tone_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_dunkle_hautfarbe_helle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_y_tono_de_piel_claro:',
+        'fr': ':poignée_de_main__peau_foncée_et_peau_claire:',
+        'ja': ':握手_濃い肌色_薄い肌色:',
+        'ko': ':악수_검은색_피부_하얀_피부:',
+        'pt': ':aperto_de_mãos_pele_escura_e_pele_clara:',
+        'it': ':stretta_di_mano_carnagione_scura_e_carnagione_chiara:',
+        'fa': ':دست_دادن_پوست_آبنوسی_پوست_سفید:',
+        'id': ':jabat_tangan_warna_kulit_gelap_warna_kulit_cerah:',
+        'zh': ':握手_较深肤色较浅肤色:'
     },
     '\U0001FAF1\U0001F3FF\U0000200D\U0001FAF2\U0001F3FE': {  # 🫱🏿‍🫲🏾
         'en': ':handshake_dark_skin_tone_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_dunkle_hautfarbe_mitteldunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_y_tono_de_piel_oscuro_medio:',
+        'fr': ':poignée_de_main__peau_foncée_et_peau_mate:',
+        'ja': ':握手_濃い肌色_やや濃い肌色:',
+        'ko': ':악수_검은색_피부_진한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_escura_e_pele_morena_escura:',
+        'it': ':stretta_di_mano_carnagione_scura_e_carnagione_abbastanza_scura:',
+        'fa': ':دست_دادن_پوست_آبنوسی_پوست_گندمی:',
+        'id': ':jabat_tangan_warna_kulit_gelap_warna_kulit_gelap-sedang:',
+        'zh': ':握手_较深肤色中等深肤色:'
     },
     '\U0001FAF1\U0001F3FF\U0000200D\U0001FAF2\U0001F3FC': {  # 🫱🏿‍🫲🏼
         'en': ':handshake_dark_skin_tone_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_dunkle_hautfarbe_mittelhelle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_y_tono_de_piel_claro_medio:',
+        'fr': ':poignée_de_main__peau_foncée_et_peau_moyennement_claire:',
+        'ja': ':握手_濃い肌色_やや薄い肌色:',
+        'ko': ':악수_검은색_피부_연한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_escura_e_pele_morena_clara:',
+        'it': ':stretta_di_mano_carnagione_scura_e_carnagione_abbastanza_chiara:',
+        'fa': ':دست_دادن_پوست_آبنوسی_پوست_روشن:',
+        'id': ':jabat_tangan_warna_kulit_gelap_warna_kulit_cerah-sedang:',
+        'zh': ':握手_较深肤色中等浅肤色:'
     },
     '\U0001FAF1\U0001F3FF\U0000200D\U0001FAF2\U0001F3FD': {  # 🫱🏿‍🫲🏽
         'en': ':handshake_dark_skin_tone_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_dunkle_hautfarbe_mittlere_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_y_tono_de_piel_medio:',
+        'fr': ':poignée_de_main__peau_foncée_et_peau_légèrement_mate:',
+        'ja': ':握手_濃い肌色_中間の肌色:',
+        'ko': ':악수_검은색_피부_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_escura_e_pele_morena:',
+        'it': ':stretta_di_mano_carnagione_scura_e_carnagione_olivastra:',
+        'fa': ':دست_دادن_پوست_آبنوسی_پوست_طلایی:',
+        'id': ':jabat_tangan_warna_kulit_gelap_warna_kulit_sedang:',
+        'zh': ':握手_较深肤色中等肤色:'
     },
     '\U0001F91D\U0001F3FB': {  # 🤝🏻
         'en': ':handshake_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_helle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro:',
+        'fr': ':poignée_de_main__peau_claire:',
+        'ja': ':握手_薄い肌色:',
+        'ko': ':악수_하얀_피부:',
+        'pt': ':aperto_de_mãos_pele_clara:',
+        'it': ':stretta_di_mano_carnagione_chiara:',
+        'fa': ':دست_دادن_پوست_سفید:',
+        'id': ':jabat_tangan_warna_kulit_cerah:',
+        'zh': ':握手_较浅肤色:'
     },
     '\U0001FAF1\U0001F3FB\U0000200D\U0001FAF2\U0001F3FF': {  # 🫱🏻‍🫲🏿
         'en': ':handshake_light_skin_tone_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_helle_hautfarbe_dunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_y_tono_de_piel_oscuro:',
+        'fr': ':poignée_de_main__peau_claire_et_peau_foncée:',
+        'ja': ':握手_薄い肌色_濃い肌色:',
+        'ko': ':악수_하얀_피부_검은색_피부:',
+        'pt': ':aperto_de_mãos_pele_clara_e_pele_escura:',
+        'it': ':stretta_di_mano_carnagione_chiara_e_carnagione_scura:',
+        'fa': ':دست_دادن_پوست_سفید_پوست_آبنوسی:',
+        'id': ':jabat_tangan_warna_kulit_cerah_warna_kulit_gelap:',
+        'zh': ':握手_较浅肤色较深肤色:'
     },
     '\U0001FAF1\U0001F3FB\U0000200D\U0001FAF2\U0001F3FE': {  # 🫱🏻‍🫲🏾
         'en': ':handshake_light_skin_tone_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_helle_hautfarbe_mitteldunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_y_tono_de_piel_oscuro_medio:',
+        'fr': ':poignée_de_main__peau_claire_et_peau_mate:',
+        'ja': ':握手_薄い肌色_やや濃い肌色:',
+        'ko': ':악수_하얀_피부_진한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_clara_e_pele_morena_escura:',
+        'it': ':stretta_di_mano_carnagione_chiara_e_carnagione_abbastanza_scura:',
+        'fa': ':دست_دادن_پوست_سفید_پوست_گندمی:',
+        'id': ':jabat_tangan_warna_kulit_cerah_warna_kulit_gelap-sedang:',
+        'zh': ':握手_较浅肤色中等深肤色:'
     },
     '\U0001FAF1\U0001F3FB\U0000200D\U0001FAF2\U0001F3FC': {  # 🫱🏻‍🫲🏼
         'en': ':handshake_light_skin_tone_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_helle_hautfarbe_mittelhelle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_y_tono_de_piel_claro_medio:',
+        'fr': ':poignée_de_main__peau_claire_et_peau_moyennement_claire:',
+        'ja': ':握手_薄い肌色_やや薄い肌色:',
+        'ko': ':악수_하얀_피부_연한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_clara_e_pele_morena_clara:',
+        'it': ':stretta_di_mano_carnagione_chiara_e_carnagione_abbastanza_chiara:',
+        'fa': ':دست_دادن_پوست_سفید_پوست_روشن:',
+        'id': ':jabat_tangan_warna_kulit_cerah_warna_kulit_cerah-sedang:',
+        'zh': ':握手_较浅肤色中等浅肤色:'
     },
     '\U0001FAF1\U0001F3FB\U0000200D\U0001FAF2\U0001F3FD': {  # 🫱🏻‍🫲🏽
         'en': ':handshake_light_skin_tone_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_helle_hautfarbe_mittlere_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_y_tono_de_piel_medio:',
+        'fr': ':poignée_de_main__peau_claire_et_peau_légèrement_mate:',
+        'ja': ':握手_薄い肌色_中間の肌色:',
+        'ko': ':악수_하얀_피부_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_clara_e_pele_morena:',
+        'it': ':stretta_di_mano_carnagione_chiara_e_carnagione_olivastra:',
+        'fa': ':دست_دادن_پوست_سفید_پوست_طلایی:',
+        'id': ':jabat_tangan_warna_kulit_cerah_warna_kulit_sedang:',
+        'zh': ':握手_较浅肤色中等肤色:'
     },
     '\U0001F91D\U0001F3FE': {  # 🤝🏾
         'en': ':handshake_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mitteldunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_medio:',
+        'fr': ':poignée_de_main__peau_mate:',
+        'ja': ':握手_やや濃い肌色:',
+        'ko': ':악수_진한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_escura:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_scura:',
+        'fa': ':دست_دادن_پوست_گندمی:',
+        'id': ':jabat_tangan_warna_kulit_gelap-sedang:',
+        'zh': ':握手_中等深肤色:'
     },
     '\U0001FAF1\U0001F3FE\U0000200D\U0001FAF2\U0001F3FF': {  # 🫱🏾‍🫲🏿
         'en': ':handshake_medium-dark_skin_tone_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mitteldunkle_hautfarbe_dunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_medio_y_tono_de_piel_oscuro:',
+        'fr': ':poignée_de_main__peau_mate_et_peau_foncée:',
+        'ja': ':握手_やや濃い肌色_濃い肌色:',
+        'ko': ':악수_진한_갈색_피부_검은색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_escura_e_pele_escura:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_scura_e_carnagione_scura:',
+        'fa': ':دست_دادن_پوست_گندمی_پوست_آبنوسی:',
+        'id': ':jabat_tangan_warna_kulit_gelap-sedang_warna_kulit_gelap:',
+        'zh': ':握手_中等深肤色较深肤色:'
     },
     '\U0001FAF1\U0001F3FE\U0000200D\U0001FAF2\U0001F3FB': {  # 🫱🏾‍🫲🏻
         'en': ':handshake_medium-dark_skin_tone_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mitteldunkle_hautfarbe_helle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_medio_y_tono_de_piel_claro:',
+        'fr': ':poignée_de_main__peau_mate_et_peau_claire:',
+        'ja': ':握手_やや濃い肌色_薄い肌色:',
+        'ko': ':악수_진한_갈색_피부_하얀_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_escura_e_pele_clara:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_scura_e_carnagione_chiara:',
+        'fa': ':دست_دادن_پوست_گندمی_پوست_سفید:',
+        'id': ':jabat_tangan_warna_kulit_gelap-sedang_warna_kulit_cerah:',
+        'zh': ':握手_中等深肤色较浅肤色:'
     },
     '\U0001FAF1\U0001F3FE\U0000200D\U0001FAF2\U0001F3FC': {  # 🫱🏾‍🫲🏼
         'en': ':handshake_medium-dark_skin_tone_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mitteldunkle_hautfarbe_mittelhelle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_medio_y_tono_de_piel_claro_medio:',
+        'fr': ':poignée_de_main__peau_mate_et_peau_moyennement_claire:',
+        'ja': ':握手_やや濃い肌色_やや薄い肌色:',
+        'ko': ':악수_진한_갈색_피부_연한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_escura_e_pele_morena_clara:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_scura_e_carnagione_abbastanza_chiara:',
+        'fa': ':دست_دادن_پوست_گندمی_پوست_روشن:',
+        'id': ':jabat_tangan_warna_kulit_gelap-sedang_warna_kulit_cerah-sedang:',
+        'zh': ':握手_中等深肤色中等浅肤色:'
     },
     '\U0001FAF1\U0001F3FE\U0000200D\U0001FAF2\U0001F3FD': {  # 🫱🏾‍🫲🏽
         'en': ':handshake_medium-dark_skin_tone_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mitteldunkle_hautfarbe_mittlere_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_oscuro_medio_y_tono_de_piel_medio:',
+        'fr': ':poignée_de_main__peau_mate_et_peau_légèrement_mate:',
+        'ja': ':握手_やや濃い肌色_中間の肌色:',
+        'ko': ':악수_진한_갈색_피부_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_escura_e_pele_morena:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_scura_e_carnagione_olivastra:',
+        'fa': ':دست_دادن_پوست_گندمی_پوست_طلایی:',
+        'id': ':jabat_tangan_warna_kulit_gelap-sedang_warna_kulit_sedang:',
+        'zh': ':握手_中等深肤色中等肤色:'
     },
     '\U0001F91D\U0001F3FC': {  # 🤝🏼
         'en': ':handshake_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittelhelle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_medio:',
+        'fr': ':poignée_de_main__peau_moyennement_claire:',
+        'ja': ':握手_やや薄い肌色:',
+        'ko': ':악수_연한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_clara:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_chiara:',
+        'fa': ':دست_دادن_پوست_روشن:',
+        'id': ':jabat_tangan_warna_kulit_cerah-sedang:',
+        'zh': ':握手_中等浅肤色:'
     },
     '\U0001FAF1\U0001F3FC\U0000200D\U0001FAF2\U0001F3FF': {  # 🫱🏼‍🫲🏿
         'en': ':handshake_medium-light_skin_tone_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittelhelle_hautfarbe_dunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_medio_y_tono_de_piel_oscuro:',
+        'fr': ':poignée_de_main__peau_moyennement_claire_et_peau_foncée:',
+        'ja': ':握手_やや薄い肌色_濃い肌色:',
+        'ko': ':악수_연한_갈색_피부_검은색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_clara_e_pele_escura:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_chiara_e_carnagione_scura:',
+        'fa': ':دست_دادن_پوست_روشن_پوست_آبنوسی:',
+        'id': ':jabat_tangan_warna_kulit_cerah-sedang_warna_kulit_gelap:',
+        'zh': ':握手_中等浅肤色较深肤色:'
     },
     '\U0001FAF1\U0001F3FC\U0000200D\U0001FAF2\U0001F3FB': {  # 🫱🏼‍🫲🏻
         'en': ':handshake_medium-light_skin_tone_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittelhelle_hautfarbe_helle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_medio_y_tono_de_piel_claro:',
+        'fr': ':poignée_de_main__peau_moyennement_claire_et_peau_claire:',
+        'ja': ':握手_やや薄い肌色_薄い肌色:',
+        'ko': ':악수_연한_갈색_피부_하얀_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_clara_e_pele_clara:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_chiara_e_carnagione_chiara:',
+        'fa': ':دست_دادن_پوست_روشن_پوست_سفید:',
+        'id': ':jabat_tangan_warna_kulit_cerah-sedang_warna_kulit_cerah:',
+        'zh': ':握手_中等浅肤色较浅肤色:'
     },
     '\U0001FAF1\U0001F3FC\U0000200D\U0001FAF2\U0001F3FE': {  # 🫱🏼‍🫲🏾
         'en': ':handshake_medium-light_skin_tone_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittelhelle_hautfarbe_mitteldunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_medio_y_tono_de_piel_oscuro_medio:',
+        'fr': ':poignée_de_main__peau_moyennement_claire_et_peau_mate:',
+        'ja': ':握手_やや薄い肌色_やや濃い肌色:',
+        'ko': ':악수_연한_갈색_피부_진한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_clara_e_pele_morena_escura:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_chiara_e_carnagione_abbastanza_scura:',
+        'fa': ':دست_دادن_پوست_روشن_پوست_گندمی:',
+        'id': ':jabat_tangan_warna_kulit_cerah-sedang_warna_kulit_gelap-sedang:',
+        'zh': ':握手_中等浅肤色中等深肤色:'
     },
     '\U0001FAF1\U0001F3FC\U0000200D\U0001FAF2\U0001F3FD': {  # 🫱🏼‍🫲🏽
         'en': ':handshake_medium-light_skin_tone_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittelhelle_hautfarbe_mittlere_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_claro_medio_y_tono_de_piel_medio:',
+        'fr': ':poignée_de_main__peau_moyennement_claire_et_peau_légèrement_mate:',
+        'ja': ':握手_やや薄い肌色_中間の肌色:',
+        'ko': ':악수_연한_갈색_피부_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_clara_e_pele_morena:',
+        'it': ':stretta_di_mano_carnagione_abbastanza_chiara_e_carnagione_olivastra:',
+        'fa': ':دست_دادن_پوست_روشن_پوست_طلایی:',
+        'id': ':jabat_tangan_warna_kulit_cerah-sedang_warna_kulit_sedang:',
+        'zh': ':握手_中等浅肤色中等肤色:'
     },
     '\U0001F91D\U0001F3FD': {  # 🤝🏽
         'en': ':handshake_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittlere_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_medio:',
+        'fr': ':poignée_de_main__peau_légèrement_mate:',
+        'ja': ':握手_中間の肌色:',
+        'ko': ':악수_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena:',
+        'it': ':stretta_di_mano_carnagione_olivastra:',
+        'fa': ':دست_دادن_پوست_طلایی:',
+        'id': ':jabat_tangan_warna_kulit_sedang:',
+        'zh': ':握手_中等肤色:'
     },
     '\U0001FAF1\U0001F3FD\U0000200D\U0001FAF2\U0001F3FF': {  # 🫱🏽‍🫲🏿
         'en': ':handshake_medium_skin_tone_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittlere_hautfarbe_dunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_medio_y_tono_de_piel_oscuro:',
+        'fr': ':poignée_de_main__peau_légèrement_mate_et_peau_foncée:',
+        'ja': ':握手_中間の肌色_濃い肌色:',
+        'ko': ':악수_갈색_피부_검은색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_e_pele_escura:',
+        'it': ':stretta_di_mano_carnagione_olivastra_e_carnagione_scura:',
+        'fa': ':دست_دادن_پوست_طلایی_پوست_آبنوسی:',
+        'id': ':jabat_tangan_warna_kulit_sedang_warna_kulit_gelap:',
+        'zh': ':握手_中等肤色较深肤色:'
     },
     '\U0001FAF1\U0001F3FD\U0000200D\U0001FAF2\U0001F3FB': {  # 🫱🏽‍🫲🏻
         'en': ':handshake_medium_skin_tone_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittlere_hautfarbe_helle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_medio_y_tono_de_piel_claro:',
+        'fr': ':poignée_de_main__peau_légèrement_mate_et_peau_claire:',
+        'ja': ':握手_中間の肌色_薄い肌色:',
+        'ko': ':악수_갈색_피부_하얀_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_e_pele_clara:',
+        'it': ':stretta_di_mano_carnagione_olivastra_e_carnagione_chiara:',
+        'fa': ':دست_دادن_پوست_طلایی_پوست_سفید:',
+        'id': ':jabat_tangan_warna_kulit_sedang_warna_kulit_cerah:',
+        'zh': ':握手_中等肤色较浅肤色:'
     },
     '\U0001FAF1\U0001F3FD\U0000200D\U0001FAF2\U0001F3FE': {  # 🫱🏽‍🫲🏾
         'en': ':handshake_medium_skin_tone_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittlere_hautfarbe_mitteldunkle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_medio_y_tono_de_piel_oscuro_medio:',
+        'fr': ':poignée_de_main__peau_légèrement_mate_et_peau_mate:',
+        'ja': ':握手_中間の肌色_やや濃い肌色:',
+        'ko': ':악수_갈색_피부_진한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_e_pele_morena_escura:',
+        'it': ':stretta_di_mano_carnagione_olivastra_e_carnagione_abbastanza_scura:',
+        'fa': ':دست_دادن_پوست_طلایی_پوست_گندمی:',
+        'id': ':jabat_tangan_warna_kulit_sedang_warna_kulit_gelap-sedang:',
+        'zh': ':握手_中等肤色中等深肤色:'
     },
     '\U0001FAF1\U0001F3FD\U0000200D\U0001FAF2\U0001F3FC': {  # 🫱🏽‍🫲🏼
         'en': ':handshake_medium_skin_tone_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':handschlag_mittlere_hautfarbe_mittelhelle_hautfarbe:',
+        'es': ':apretón_de_manos_tono_de_piel_medio_y_tono_de_piel_claro_medio:',
+        'fr': ':poignée_de_main__peau_légèrement_mate_et_peau_moyennement_claire:',
+        'ja': ':握手_中間の肌色_やや薄い肌色:',
+        'ko': ':악수_갈색_피부_연한_갈색_피부:',
+        'pt': ':aperto_de_mãos_pele_morena_e_pele_morena_clara:',
+        'it': ':stretta_di_mano_carnagione_olivastra_e_carnagione_abbastanza_chiara:',
+        'fa': ':دست_دادن_پوست_طلایی_پوست_روشن:',
+        'id': ':jabat_tangan_warna_kulit_sedang_warna_kulit_cerah-sedang:',
+        'zh': ':握手_中等肤色中等浅肤色:'
     },
     '\U0001F423': {  # 🐣
         'en': ':hatching_chick:',
         'status': fully_qualified,
         'E': 0.6,
         'de': ':schlüpfendes_küken:',
         'es': ':pollito_rompiendo_el_cascarón:',
@@ -20478,15 +20804,15 @@
         'id': ':petugas_kesehatan_warna_kulit_sedang:',
         'zh': ':卫生工作者_中等肤色:'
     },
     '\U0001F649': {  # 🙉
         'en': ':hear-no-evil_monkey:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':hear_no_evil:'],
+        'alias': [':hear_no_evil:', ':hear_no_evil_monkey:'],
         'de': ':sich_die_ohren_zuhaltendes_affengesicht:',
         'es': ':mono_con_los_oídos_tapados:',
         'fr': ':singe_ne_rien_entendre:',
         'ja': ':聞かざる:',
         'ko': ':귀를_막고_있는_원숭이:',
         'pt': ':macaco_que_não_ouve_nada:',
         'it': ':non_sento:',
@@ -20557,35 +20883,85 @@
         'fa': ':شکل_قلب_با_دست:',
         'id': ':tangan_membentuk_hati:',
         'zh': ':做成心形的双手:'
     },
     '\U0001FAF6\U0001F3FF': {  # 🫶🏿
         'en': ':heart_hands_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hände_die_herz_bilden_dunkle_hautfarbe:',
+        'es': ':manos_formando_un_corazón_tono_de_piel_oscuro:',
+        'fr': ':mains_qui_forment_un_cœur__peau_foncée:',
+        'ja': ':ハート形の手_濃い肌色:',
+        'ko': ':손_하트_검은색_피부:',
+        'pt': ':mãos_de_coração_pele_escura:',
+        'it': ':mani_a_cuore_carnagione_scura:',
+        'fa': ':شکل_قلب_با_دست_پوست_آبنوسی:',
+        'id': ':tangan_membentuk_hati_warna_kulit_gelap:',
+        'zh': ':做成心形的双手_较深肤色:'
     },
     '\U0001FAF6\U0001F3FB': {  # 🫶🏻
         'en': ':heart_hands_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hände_die_herz_bilden_helle_hautfarbe:',
+        'es': ':manos_formando_un_corazón_tono_de_piel_claro:',
+        'fr': ':mains_qui_forment_un_cœur__peau_claire:',
+        'ja': ':ハート形の手_薄い肌色:',
+        'ko': ':손_하트_하얀_피부:',
+        'pt': ':mãos_de_coração_pele_clara:',
+        'it': ':mani_a_cuore_carnagione_chiara:',
+        'fa': ':شکل_قلب_با_دست_پوست_سفید:',
+        'id': ':tangan_membentuk_hati_warna_kulit_cerah:',
+        'zh': ':做成心形的双手_较浅肤色:'
     },
     '\U0001FAF6\U0001F3FE': {  # 🫶🏾
         'en': ':heart_hands_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hände_die_herz_bilden_mitteldunkle_hautfarbe:',
+        'es': ':manos_formando_un_corazón_tono_de_piel_oscuro_medio:',
+        'fr': ':mains_qui_forment_un_cœur__peau_mate:',
+        'ja': ':ハート形の手_やや濃い肌色:',
+        'ko': ':손_하트_진한_갈색_피부:',
+        'pt': ':mãos_de_coração_pele_morena_escura:',
+        'it': ':mani_a_cuore_carnagione_abbastanza_scura:',
+        'fa': ':شکل_قلب_با_دست_پوست_گندمی:',
+        'id': ':tangan_membentuk_hati_warna_kulit_gelap-sedang:',
+        'zh': ':做成心形的双手_中等深肤色:'
     },
     '\U0001FAF6\U0001F3FC': {  # 🫶🏼
         'en': ':heart_hands_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hände_die_herz_bilden_mittelhelle_hautfarbe:',
+        'es': ':manos_formando_un_corazón_tono_de_piel_claro_medio:',
+        'fr': ':mains_qui_forment_un_cœur__peau_moyennement_claire:',
+        'ja': ':ハート形の手_やや薄い肌色:',
+        'ko': ':손_하트_연한_갈색_피부:',
+        'pt': ':mãos_de_coração_pele_morena_clara:',
+        'it': ':mani_a_cuore_carnagione_abbastanza_chiara:',
+        'fa': ':شکل_قلب_با_دست_پوست_روشن:',
+        'id': ':tangan_membentuk_hati_warna_kulit_cerah-sedang:',
+        'zh': ':做成心形的双手_中等浅肤色:'
     },
     '\U0001FAF6\U0001F3FD': {  # 🫶🏽
         'en': ':heart_hands_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hände_die_herz_bilden_mittlere_hautfarbe:',
+        'es': ':manos_formando_un_corazón_tono_de_piel_medio:',
+        'fr': ':mains_qui_forment_un_cœur__peau_légèrement_mate:',
+        'ja': ':ハート形の手_中間の肌色:',
+        'ko': ':손_하트_갈색_피부:',
+        'pt': ':mãos_de_coração_pele_morena:',
+        'it': ':mani_a_cuore_carnagione_olivastra:',
+        'fa': ':شکل_قلب_با_دست_پوست_طلایی:',
+        'id': ':tangan_membentuk_hati_warna_kulit_sedang:',
+        'zh': ':做成心形的双手_中等肤色:'
     },
     '\U00002764\U0000FE0F\U0000200D\U0001F525': {  # ❤️‍🔥
         'en': ':heart_on_fire:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':herz_in_flammen:',
         'es': ':corazón_en_llamas:',
@@ -20769,15 +21145,15 @@
         'id': ':kembang_sepatu:',
         'zh': ':芙蓉:'
     },
     '\U0001F460': {  # 👠
         'en': ':high-heeled_shoe:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':high_heel:'],
+        'alias': [':high_heel:', ':high_heeled_shoe:'],
         'de': ':stöckelschuh:',
         'es': ':zapato_de_tacón:',
         'fr': ':chaussure_à_talon_haut:',
         'ja': ':ハイヒール:',
         'ko': ':하이힐:',
         'pt': ':sapato_de_salto_alto:',
         'it': ':scarpa_con_il_tacco:',
@@ -20785,15 +21161,15 @@
         'id': ':sepatu_hak_tinggi:',
         'zh': ':高跟鞋:'
     },
     '\U0001F684': {  # 🚄
         'en': ':high-speed_train:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':bullettrain_side:'],
+        'alias': [':bullettrain_side:', ':high_speed_train:'],
         'de': ':hochgeschwindigkeitszug_mit_spitzer_nase:',
         'es': ':tren_de_alta_velocidad:',
         'fr': ':tgv:',
         'ja': ':新幹線:',
         'ko': ':고속열차:',
         'pt': ':trem_de_alta_velocidade:',
         'it': ':treno_alta_velocità:',
@@ -21540,35 +21916,85 @@
         'fa': ':اشاره_به_بیننده:',
         'id': ':jari_telunjuk_menunjuk_penonton:',
         'zh': ':指向观察者的食指:'
     },
     '\U0001FAF5\U0001F3FF': {  # 🫵🏿
         'en': ':index_pointing_at_the_viewer_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':auf_betrachter_zeigender_zeigefinger_dunkle_hautfarbe:',
+        'es': ':dedo_índice_apuntándote_a_ti_tono_de_piel_oscuro:',
+        'fr': ':index_pointant_vers_l’utilisateur__peau_foncée:',
+        'ja': ':人を指差している手_濃い肌色:',
+        'ko': ':보는_사람을_가리키는_검지_검은색_피부:',
+        'pt': ':indicador_apontando_para_o_visualizador_pele_escura:',
+        'it': ':indice_verso_l’osservatore_carnagione_scura:',
+        'fa': ':اشاره_به_بیننده_پوست_آبنوسی:',
+        'id': ':jari_telunjuk_menunjuk_penonton_warna_kulit_gelap:',
+        'zh': ':指向观察者的食指_较深肤色:'
     },
     '\U0001FAF5\U0001F3FB': {  # 🫵🏻
         'en': ':index_pointing_at_the_viewer_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':auf_betrachter_zeigender_zeigefinger_helle_hautfarbe:',
+        'es': ':dedo_índice_apuntándote_a_ti_tono_de_piel_claro:',
+        'fr': ':index_pointant_vers_l’utilisateur__peau_claire:',
+        'ja': ':人を指差している手_薄い肌色:',
+        'ko': ':보는_사람을_가리키는_검지_하얀_피부:',
+        'pt': ':indicador_apontando_para_o_visualizador_pele_clara:',
+        'it': ':indice_verso_l’osservatore_carnagione_chiara:',
+        'fa': ':اشاره_به_بیننده_پوست_سفید:',
+        'id': ':jari_telunjuk_menunjuk_penonton_warna_kulit_cerah:',
+        'zh': ':指向观察者的食指_较浅肤色:'
     },
     '\U0001FAF5\U0001F3FE': {  # 🫵🏾
         'en': ':index_pointing_at_the_viewer_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':auf_betrachter_zeigender_zeigefinger_mitteldunkle_hautfarbe:',
+        'es': ':dedo_índice_apuntándote_a_ti_tono_de_piel_oscuro_medio:',
+        'fr': ':index_pointant_vers_l’utilisateur__peau_mate:',
+        'ja': ':人を指差している手_やや濃い肌色:',
+        'ko': ':보는_사람을_가리키는_검지_진한_갈색_피부:',
+        'pt': ':indicador_apontando_para_o_visualizador_pele_morena_escura:',
+        'it': ':indice_verso_l’osservatore_carnagione_abbastanza_scura:',
+        'fa': ':اشاره_به_بیننده_پوست_گندمی:',
+        'id': ':jari_telunjuk_menunjuk_penonton_warna_kulit_gelap-sedang:',
+        'zh': ':指向观察者的食指_中等深肤色:'
     },
     '\U0001FAF5\U0001F3FC': {  # 🫵🏼
         'en': ':index_pointing_at_the_viewer_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':auf_betrachter_zeigender_zeigefinger_mittelhelle_hautfarbe:',
+        'es': ':dedo_índice_apuntándote_a_ti_tono_de_piel_claro_medio:',
+        'fr': ':index_pointant_vers_l’utilisateur__peau_moyennement_claire:',
+        'ja': ':人を指差している手_やや薄い肌色:',
+        'ko': ':보는_사람을_가리키는_검지_연한_갈색_피부:',
+        'pt': ':indicador_apontando_para_o_visualizador_pele_morena_clara:',
+        'it': ':indice_verso_l’osservatore_carnagione_abbastanza_chiara:',
+        'fa': ':اشاره_به_بیننده_پوست_روشن:',
+        'id': ':jari_telunjuk_menunjuk_penonton_warna_kulit_cerah-sedang:',
+        'zh': ':指向观察者的食指_中等浅肤色:'
     },
     '\U0001FAF5\U0001F3FD': {  # 🫵🏽
         'en': ':index_pointing_at_the_viewer_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':auf_betrachter_zeigender_zeigefinger_mittlere_hautfarbe:',
+        'es': ':dedo_índice_apuntándote_a_ti_tono_de_piel_medio:',
+        'fr': ':index_pointant_vers_l’utilisateur__peau_légèrement_mate:',
+        'ja': ':人を指差している手_中間の肌色:',
+        'ko': ':보는_사람을_가리키는_검지_갈색_피부:',
+        'pt': ':indicador_apontando_para_o_visualizador_pele_morena:',
+        'it': ':indice_verso_l’osservatore_carnagione_olivastra:',
+        'fa': ':اشاره_به_بیننده_پوست_طلایی:',
+        'id': ':jari_telunjuk_menunjuk_penonton_warna_kulit_sedang:',
+        'zh': ':指向观察者的食指_中等肤色:'
     },
     '\U0000261D\U0000FE0F': {  # ☝️
         'en': ':index_pointing_up:',
         'status': fully_qualified,
         'E': 0.6,
         'alias': [':point_up:'],
         'variant': True,
@@ -22531,26 +22957,36 @@
     '\U0001F48F\U0001F3FF': {  # 💏🏿
         'en': ':kiss_dark_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_dunkle_hautfarbe:',
         'es': ':beso_tono_de_piel_oscuro:',
         'fr': ':bisou__peau_foncée:',
+        'ja': ':2人でキス_濃い肌色:',
+        'ko': ':키스_검은색_피부:',
         'pt': ':beijo_pele_escura:',
-        'it': ':bacio_tra_coppia_carnagione_scura:'
+        'it': ':bacio_tra_coppia_carnagione_scura:',
+        'fa': ':بوسه_پوست_آبنوسی:',
+        'id': ':berciuman_warna_kulit_gelap:',
+        'zh': ':亲吻_较深肤色:'
     },
     '\U0001F48F\U0001F3FB': {  # 💏🏻
         'en': ':kiss_light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_helle_hautfarbe:',
         'es': ':beso_tono_de_piel_claro:',
         'fr': ':bisou__peau_claire:',
+        'ja': ':2人でキス_薄い肌色:',
+        'ko': ':키스_하얀_피부:',
         'pt': ':beijo_pele_clara:',
-        'it': ':bacio_tra_coppia_carnagione_chiara:'
+        'it': ':bacio_tra_coppia_carnagione_chiara:',
+        'fa': ':بوسه_پوست_سفید:',
+        'id': ':berciuman_warna_kulit_cerah:',
+        'zh': ':亲吻_较浅肤色:'
     },
     '\U0001F468\U0000200D\U00002764\U0000FE0F\U0000200D\U0001F48B\U0000200D\U0001F468': {  # 👨‍❤️‍💋‍👨
         'en': ':kiss_man_man:',
         'status': fully_qualified,
         'E': 2,
         'alias': [':couplekiss_man_man:'],
         'de': ':sich_küssendes_paar_mann,_mann:',
@@ -23089,36 +23525,51 @@
     '\U0001F48F\U0001F3FE': {  # 💏🏾
         'en': ':kiss_medium-dark_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_mitteldunkle_hautfarbe:',
         'es': ':beso_tono_de_piel_oscuro_medio:',
         'fr': ':bisou__peau_mate:',
+        'ja': ':2人でキス_やや濃い肌色:',
+        'ko': ':키스_진한_갈색_피부:',
         'pt': ':beijo_pele_morena_escura:',
-        'it': ':bacio_tra_coppia_carnagione_abbastanza_scura:'
+        'it': ':bacio_tra_coppia_carnagione_abbastanza_scura:',
+        'fa': ':بوسه_پوست_گندمی:',
+        'id': ':berciuman_warna_kulit_gelap-sedang:',
+        'zh': ':亲吻_中等深肤色:'
     },
     '\U0001F48F\U0001F3FC': {  # 💏🏼
         'en': ':kiss_medium-light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_mittelhelle_hautfarbe:',
         'es': ':beso_tono_de_piel_claro_medio:',
         'fr': ':bisou__peau_moyennement_claire:',
+        'ja': ':2人でキス_やや薄い肌色:',
+        'ko': ':키스_연한_갈색_피부:',
         'pt': ':beijo_pele_morena_clara:',
-        'it': ':bacio_tra_coppia_carnagione_abbastanza_chiara:'
+        'it': ':bacio_tra_coppia_carnagione_abbastanza_chiara:',
+        'fa': ':بوسه_پوست_روشن:',
+        'id': ':berciuman_warna_kulit_cerah-sedang:',
+        'zh': ':亲吻_中等浅肤色:'
     },
     '\U0001F48F\U0001F3FD': {  # 💏🏽
         'en': ':kiss_medium_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_mittlere_hautfarbe:',
         'es': ':beso_tono_de_piel_medio:',
         'fr': ':bisou__peau_légèrement_mate:',
+        'ja': ':2人でキス_中間の肌色:',
+        'ko': ':키스_갈색_피부:',
         'pt': ':beijo_pele_morena:',
-        'it': ':bacio_tra_coppia_carnagione_olivastra:'
+        'it': ':bacio_tra_coppia_carnagione_olivastra:',
+        'fa': ':بوسه_پوست_طلایی:',
+        'id': ':berciuman_warna_kulit_sedang:',
+        'zh': ':亲吻_中等肤色:'
     },
     '\U0001F9D1\U0001F3FF\U0000200D\U00002764\U0000FE0F\U0000200D\U0001F48B\U0000200D\U0001F9D1\U0001F3FB': {  # 🧑🏿‍❤️‍💋‍🧑🏻
         'en': ':kiss_person_person_dark_skin_tone_light_skin_tone:',
         'status': fully_qualified,
         'E': 13.1,
         'de': ':sich_küssendes_paar_erwachsener_erwachsener_dunkle_hautfarbe,helle_hautfarbe:',
         'es': ':beso_persona_adulta_persona_adulta_tono_de_piel_oscuro_tono_de_piel_claro:',
@@ -24871,15 +25322,15 @@
         'id': ':wajah_bulan_perbani_akhir:',
         'zh': ':微笑的下弦月:'
     },
     '\U000023EE\U0000FE0F': {  # ⏮️
         'en': ':last_track_button:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':previous_track_button:', ':black_left__pointing_double_triangle_with_vertical_bar:'],
+        'alias': [':previous_track_button:', ':black_left__pointing_double_triangle_with_vertical_bar:', ':black_left_pointing_double_triangle_with_vertical_bar:'],
         'variant': True,
         'de': ':vorheriger_titel:',
         'es': ':pista_anterior:',
         'fr': ':bouton_piste_précédente:',
         'ja': ':前の曲ボタン:',
         'ko': ':마지막_트랙_버튼:',
         'pt': ':botão_de_faixa_anterior:',
@@ -24888,15 +25339,15 @@
         'id': ':tombol_lagu_terakhir:',
         'zh': ':上一个音轨按钮:'
     },
     '\U000023EE': {  # ⏮
         'en': ':last_track_button:',
         'status': unqualified,
         'E': 0.7,
-        'alias': [':previous_track_button:', ':black_left__pointing_double_triangle_with_vertical_bar:'],
+        'alias': [':previous_track_button:', ':black_left__pointing_double_triangle_with_vertical_bar:', ':black_left_pointing_double_triangle_with_vertical_bar:'],
         'variant': True,
         'de': ':vorheriger_titel:',
         'es': ':pista_anterior:',
         'fr': ':bouton_piste_précédente:',
         'ja': ':前の曲ボタン:',
         'ko': ':마지막_트랙_버튼:',
         'pt': ':botão_de_faixa_anterior:',
@@ -24983,15 +25434,15 @@
         'id': ':buku_besar:',
         'zh': ':账本:'
     },
     '\U0001F91B': {  # 🤛
         'en': ':left-facing_fist:',
         'status': fully_qualified,
         'E': 3,
-        'alias': [':fist_left:'],
+        'alias': [':fist_left:', ':left_facing_fist:'],
         'de': ':faust_nach_links:',
         'es': ':puño_hacia_la_izquierda:',
         'fr': ':poing_à_gauche:',
         'ja': ':左向きのこぶし:',
         'ko': ':왼쪽을_향하는_주먹:',
         'pt': ':punho_esquerdo:',
         'it': ':pugno_a_sinistra:',
@@ -25237,35 +25688,85 @@
         'fa': ':دست_به_سمت_چپ:',
         'id': ':tangan_menghadap_kiri:',
         'zh': ':向左的手:'
     },
     '\U0001FAF2\U0001F3FF': {  # 🫲🏿
         'en': ':leftwards_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_links_weisende_hand_dunkle_hautfarbe:',
+        'es': ':mano_hacia_la_izquierda_tono_de_piel_oscuro:',
+        'fr': ':main_vers_la_gauche__peau_foncée:',
+        'ja': ':左に向けた手_濃い肌色:',
+        'ko': ':왼쪽으로_향하는_손바닥_검은색_피부:',
+        'pt': ':mão_para_a_esquerda_pele_escura:',
+        'it': ':mano_rivolta_a_sinistra_carnagione_scura:',
+        'fa': ':دست_به_سمت_چپ_پوست_آبنوسی:',
+        'id': ':tangan_menghadap_kiri_warna_kulit_gelap:',
+        'zh': ':向左的手_较深肤色:'
     },
     '\U0001FAF2\U0001F3FB': {  # 🫲🏻
         'en': ':leftwards_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_links_weisende_hand_helle_hautfarbe:',
+        'es': ':mano_hacia_la_izquierda_tono_de_piel_claro:',
+        'fr': ':main_vers_la_gauche__peau_claire:',
+        'ja': ':左に向けた手_薄い肌色:',
+        'ko': ':왼쪽으로_향하는_손바닥_하얀_피부:',
+        'pt': ':mão_para_a_esquerda_pele_clara:',
+        'it': ':mano_rivolta_a_sinistra_carnagione_chiara:',
+        'fa': ':دست_به_سمت_چپ_پوست_سفید:',
+        'id': ':tangan_menghadap_kiri_warna_kulit_cerah:',
+        'zh': ':向左的手_较浅肤色:'
     },
     '\U0001FAF2\U0001F3FE': {  # 🫲🏾
         'en': ':leftwards_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_links_weisende_hand_mitteldunkle_hautfarbe:',
+        'es': ':mano_hacia_la_izquierda_tono_de_piel_oscuro_medio:',
+        'fr': ':main_vers_la_gauche__peau_mate:',
+        'ja': ':左に向けた手_やや濃い肌色:',
+        'ko': ':왼쪽으로_향하는_손바닥_진한_갈색_피부:',
+        'pt': ':mão_para_a_esquerda_pele_morena_escura:',
+        'it': ':mano_rivolta_a_sinistra_carnagione_abbastanza_scura:',
+        'fa': ':دست_به_سمت_چپ_پوست_گندمی:',
+        'id': ':tangan_menghadap_kiri_warna_kulit_gelap-sedang:',
+        'zh': ':向左的手_中等深肤色:'
     },
     '\U0001FAF2\U0001F3FC': {  # 🫲🏼
         'en': ':leftwards_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_links_weisende_hand_mittelhelle_hautfarbe:',
+        'es': ':mano_hacia_la_izquierda_tono_de_piel_claro_medio:',
+        'fr': ':main_vers_la_gauche__peau_moyennement_claire:',
+        'ja': ':左に向けた手_やや薄い肌色:',
+        'ko': ':왼쪽으로_향하는_손바닥_연한_갈색_피부:',
+        'pt': ':mão_para_a_esquerda_pele_morena_clara:',
+        'it': ':mano_rivolta_a_sinistra_carnagione_abbastanza_chiara:',
+        'fa': ':دست_به_سمت_چپ_پوست_روشن:',
+        'id': ':tangan_menghadap_kiri_warna_kulit_cerah-sedang:',
+        'zh': ':向左的手_中等浅肤色:'
     },
     '\U0001FAF2\U0001F3FD': {  # 🫲🏽
         'en': ':leftwards_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_links_weisende_hand_mittlere_hautfarbe:',
+        'es': ':mano_hacia_la_izquierda_tono_de_piel_medio:',
+        'fr': ':main_vers_la_gauche__peau_légèrement_mate:',
+        'ja': ':左に向けた手_中間の肌色:',
+        'ko': ':왼쪽으로_향하는_손바닥_갈색_피부:',
+        'pt': ':mão_para_a_esquerda_pele_morena:',
+        'it': ':mano_rivolta_a_sinistra_carnagione_olivastra:',
+        'fa': ':دست_به_سمت_چپ_پوست_طلایی:',
+        'id': ':tangan_menghadap_kiri_warna_kulit_sedang:',
+        'zh': ':向左的手_中等肤色:'
     },
     '\U0001FAF7': {  # 🫷
         'en': ':leftwards_pushing_hand:',
         'status': fully_qualified,
         'E': 15,
         'de': ':nach_links_schiebende_hand:',
         'es': ':mano_empujando_hacia_la_izquierda:',
@@ -25277,35 +25778,85 @@
         'fa': ':دست_فشاردهنده_به_سمت_چپ:',
         'id': ':tangan_mendorong_ke_kiri:',
         'zh': ':向左推:'
     },
     '\U0001FAF7\U0001F3FF': {  # 🫷🏿
         'en': ':leftwards_pushing_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_links_schiebende_hand_dunkle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_izquierda_tono_de_piel_oscuro:',
+        'fr': ':main_qui_pousse_vers_la_gauche__peau_foncée:',
+        'ja': ':左向きに押している手_濃い肌色:',
+        'ko': ':왼쪽으로_밀치는_손_검은색_피부:',
+        'pt': ':mão_empurrando_para_a_esquerda_pele_escura:',
+        'it': ':mano_che_spinge_a_sinistra_carnagione_scura:',
+        'fa': ':دست_فشاردهنده_به_سمت_چپ_پوست_آبنوسی:',
+        'id': ':tangan_mendorong_ke_kiri_warna_kulit_gelap:',
+        'zh': ':向左推_较深肤色:'
     },
     '\U0001FAF7\U0001F3FB': {  # 🫷🏻
         'en': ':leftwards_pushing_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_links_schiebende_hand_helle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_izquierda_tono_de_piel_claro:',
+        'fr': ':main_qui_pousse_vers_la_gauche__peau_claire:',
+        'ja': ':左向きに押している手_薄い肌色:',
+        'ko': ':왼쪽으로_밀치는_손_하얀_피부:',
+        'pt': ':mão_empurrando_para_a_esquerda_pele_clara:',
+        'it': ':mano_che_spinge_a_sinistra_carnagione_chiara:',
+        'fa': ':دست_فشاردهنده_به_سمت_چپ_پوست_سفید:',
+        'id': ':tangan_mendorong_ke_kiri_warna_kulit_cerah:',
+        'zh': ':向左推_较浅肤色:'
     },
     '\U0001FAF7\U0001F3FE': {  # 🫷🏾
         'en': ':leftwards_pushing_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_links_schiebende_hand_mitteldunkle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_izquierda_tono_de_piel_oscuro_medio:',
+        'fr': ':main_qui_pousse_vers_la_gauche__peau_mate:',
+        'ja': ':左向きに押している手_やや濃い肌色:',
+        'ko': ':왼쪽으로_밀치는_손_진한_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_esquerda_pele_morena_escura:',
+        'it': ':mano_che_spinge_a_sinistra_carnagione_abbastanza_scura:',
+        'fa': ':دست_فشاردهنده_به_سمت_چپ_پوست_گندمی:',
+        'id': ':tangan_mendorong_ke_kiri_warna_kulit_gelap-sedang:',
+        'zh': ':向左推_中等深肤色:'
     },
     '\U0001FAF7\U0001F3FC': {  # 🫷🏼
         'en': ':leftwards_pushing_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_links_schiebende_hand_mittelhelle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_izquierda_tono_de_piel_claro_medio:',
+        'fr': ':main_qui_pousse_vers_la_gauche__peau_moyennement_claire:',
+        'ja': ':左向きに押している手_やや薄い肌色:',
+        'ko': ':왼쪽으로_밀치는_손_연한_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_esquerda_pele_morena_clara:',
+        'it': ':mano_che_spinge_a_sinistra_carnagione_abbastanza_chiara:',
+        'fa': ':دست_فشاردهنده_به_سمت_چپ_پوست_روشن:',
+        'id': ':tangan_mendorong_ke_kiri_warna_kulit_cerah-sedang:',
+        'zh': ':向左推_中等浅肤色:'
     },
     '\U0001FAF7\U0001F3FD': {  # 🫷🏽
         'en': ':leftwards_pushing_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_links_schiebende_hand_mittlere_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_izquierda_tono_de_piel_medio:',
+        'fr': ':main_qui_pousse_vers_la_gauche__peau_légèrement_mate:',
+        'ja': ':左向きに押している手_中間の肌色:',
+        'ko': ':왼쪽으로_밀치는_손_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_esquerda_pele_morena:',
+        'it': ':mano_che_spinge_a_sinistra_carnagione_olivastra:',
+        'fa': ':دست_فشاردهنده_به_سمت_چپ_پوست_طلایی:',
+        'id': ':tangan_mendorong_ke_kiri_warna_kulit_sedang:',
+        'zh': ':向左推_中等肤色:'
     },
     '\U0001F9B5': {  # 🦵
         'en': ':leg:',
         'status': fully_qualified,
         'E': 11,
         'de': ':bein:',
         'es': ':pierna:',
@@ -29270,15 +29821,15 @@
         'id': ':jin_pria:',
         'zh': ':男妖怪:'
     },
     '\U0001F645\U0000200D\U00002642\U0000FE0F': {  # 🙅‍♂️
         'en': ':man_gesturing_NO:',
         'status': fully_qualified,
         'E': 4,
-        'alias': [':no_good_man:', ':ng_man:'],
+        'alias': [':no_good_man:', ':ng_man:', ':man_gesturing_no:'],
         'de': ':mann_mit_überkreuzten_armen:',
         'es': ':hombre_haciendo_el_gesto_de_no:',
         'fr': ':homme_faisant_un_geste_d’interdiction:',
         'ja': ':ダメのポーズをする男:',
         'ko': ':안_된다는_제스처를_하는_남자:',
         'pt': ':homem_fazendo_gesto_de_“não”:',
         'it': ':uomo_con_gesto_di_rifiuto:',
@@ -29286,15 +29837,15 @@
         'id': ':pria_mengisyaratkan_tidak:',
         'zh': ':禁止手势男:'
     },
     '\U0001F645\U0000200D\U00002642': {  # 🙅‍♂
         'en': ':man_gesturing_NO:',
         'status': minimally_qualified,
         'E': 4,
-        'alias': [':no_good_man:', ':ng_man:'],
+        'alias': [':no_good_man:', ':ng_man:', ':man_gesturing_no:'],
         'de': ':mann_mit_überkreuzten_armen:',
         'es': ':hombre_haciendo_el_gesto_de_no:',
         'fr': ':homme_faisant_un_geste_d’interdiction:',
         'ja': ':ダメのポーズをする男:',
         'ko': ':안_된다는_제스처를_하는_남자:',
         'pt': ':homem_fazendo_gesto_de_“não”:',
         'it': ':uomo_con_gesto_di_rifiuto:',
@@ -29452,15 +30003,15 @@
         'id': ':pria_mengisyaratkan_tidak_warna_kulit_sedang:',
         'zh': ':禁止手势男_中等肤色:'
     },
     '\U0001F646\U0000200D\U00002642\U0000FE0F': {  # 🙆‍♂️
         'en': ':man_gesturing_OK:',
         'status': fully_qualified,
         'E': 4,
-        'alias': [':ok_man:'],
+        'alias': [':ok_man:', ':man_gesturing_ok:'],
         'de': ':mann_mit_händen_auf_dem_kopf:',
         'es': ':hombre_haciendo_el_gesto_de_de_acuerdo:',
         'fr': ':homme_faisant_un_geste_d’acceptation:',
         'ja': ':okのポーズをする男:',
         'ko': ':오케이라는_제스처를_하는_남자:',
         'pt': ':homem_fazendo_gesto_de_“ok”:',
         'it': ':uomo_con_gesto_ok:',
@@ -29468,15 +30019,15 @@
         'id': ':pria_mengisyaratkan_oke:',
         'zh': ':OK手势男:'
     },
     '\U0001F646\U0000200D\U00002642': {  # 🙆‍♂
         'en': ':man_gesturing_OK:',
         'status': minimally_qualified,
         'E': 4,
-        'alias': [':ok_man:'],
+        'alias': [':ok_man:', ':man_gesturing_ok:'],
         'de': ':mann_mit_händen_auf_dem_kopf:',
         'es': ':hombre_haciendo_el_gesto_de_de_acuerdo:',
         'fr': ':homme_faisant_un_geste_d’acceptation:',
         'ja': ':okのポーズをする男:',
         'ko': ':오케이라는_제스처를_하는_남자:',
         'pt': ':homem_fazendo_gesto_de_“ok”:',
         'it': ':uomo_con_gesto_ok:',
@@ -37269,15 +37820,15 @@
         'id': ':sepatu_pria:',
         'zh': ':男鞋:'
     },
     '\U0001F5FE': {  # 🗾
         'en': ':map_of_Japan:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':japan:'],
+        'alias': [':japan:', ':map_of_japan:'],
         'de': ':umriss_von_japan:',
         'es': ':mapa_de_japón:',
         'fr': ':carte_du_japon:',
         'ja': ':日本地図:',
         'ko': ':일본_지도:',
         'pt': ':mapa_do_japão:',
         'it': ':mappa_del_giappone:',
@@ -38121,15 +38672,15 @@
         'id': ':menorah:',
         'zh': ':烛台:'
     },
     '\U0001F6B9': {  # 🚹
         'en': ':men’s_room:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':mens:'],
+        'alias': [':mens:', ':mens_room:'],
         'variant': True,
         'de': ':herren:',
         'es': ':aseo_para_hombres:',
         'fr': ':symbole_toilettes_hommes:',
         'ja': ':男子トイレ:',
         'ko': ':남자_화장실:',
         'pt': ':banheiro_masculino:',
@@ -39886,15 +40437,15 @@
         'id': ':koran:',
         'zh': ':报纸:'
     },
     '\U000023ED\U0000FE0F': {  # ⏭️
         'en': ':next_track_button:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':black_right__pointing_double_triangle_with_vertical_bar:'],
+        'alias': [':black_right__pointing_double_triangle_with_vertical_bar:', ':black_right_pointing_double_triangle_with_vertical_bar:'],
         'variant': True,
         'de': ':nächster_titel:',
         'es': ':pista_siguiente:',
         'fr': ':bouton_piste_suivante:',
         'ja': ':次の曲ボタン:',
         'ko': ':다음_트랙_버튼:',
         'pt': ':botão_de_próxima_faixa:',
@@ -39903,15 +40454,15 @@
         'id': ':tombol_lagu_berikutnya:',
         'zh': ':下一个音轨按钮:'
     },
     '\U000023ED': {  # ⏭
         'en': ':next_track_button:',
         'status': unqualified,
         'E': 0.7,
-        'alias': [':black_right__pointing_double_triangle_with_vertical_bar:'],
+        'alias': [':black_right__pointing_double_triangle_with_vertical_bar:', ':black_right_pointing_double_triangle_with_vertical_bar:'],
         'variant': True,
         'de': ':nächster_titel:',
         'es': ':pista_siguiente:',
         'fr': ':bouton_piste_suivante:',
         'ja': ':次の曲ボタン:',
         'ko': ':다음_트랙_버튼:',
         'pt': ':botão_de_próxima_faixa:',
@@ -39935,15 +40486,15 @@
         'id': ':malam_berbintang:',
         'zh': ':夜晚:'
     },
     '\U0001F564': {  # 🕤
         'en': ':nine-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock930:'],
+        'alias': [':clock930:', ':nine_thirty:'],
         'variant': True,
         'de': ':9.30_uhr:',
         'es': ':nueve_y_media:',
         'fr': ':neuf_heures_et_demie:',
         'ja': ':9時半:',
         'ko': ':아홉_시_반:',
         'pt': ':nove_e_meia:',
@@ -39952,15 +40503,15 @@
         'id': ':jam_setengah_sepuluh:',
         'zh': ':九点半:'
     },
     '\U0001F558': {  # 🕘
         'en': ':nine_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock9:'],
+        'alias': [':clock9:', ':nine_oclock:'],
         'variant': True,
         'de': ':9.00_uhr:',
         'es': ':9_en_punto:',
         'fr': ':neuf_heures:',
         'ja': ':9時:',
         'ko': ':아홉_시:',
         'pt': ':9_horas:',
@@ -40168,15 +40719,15 @@
         'id': ':dilarang_merokok:',
         'zh': ':禁止吸烟:'
     },
     '\U0001F6B1': {  # 🚱
         'en': ':non-potable_water:',
         'status': fully_qualified,
         'E': 1,
-        'alias': [':non__potable_water:'],
+        'alias': [':non__potable_water:', ':non_potable_water:'],
         'de': ':kein_trinkwasser:',
         'es': ':agua_no_potable:',
         'fr': ':eau_non_potable:',
         'ja': ':飲用不可:',
         'ko': ':마실_수_없는_물:',
         'pt': ':água_não_potável:',
         'it': ':simbolo_di_acqua_non_potabile:',
@@ -41027,15 +41578,15 @@
         'id': ':pakaian_renang_one-piece:',
         'zh': ':连体泳衣:'
     },
     '\U0001F55C': {  # 🕜
         'en': ':one-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock130:'],
+        'alias': [':clock130:', ':one_thirty:'],
         'variant': True,
         'de': ':1.30_uhr:',
         'es': ':una_y_media:',
         'fr': ':une_heure_et_demie:',
         'ja': ':1時半:',
         'ko': ':한_시_반:',
         'pt': ':uma_e_meia:',
@@ -41044,15 +41595,15 @@
         'id': ':jam_setengah_dua:',
         'zh': ':一点半:'
     },
     '\U0001F550': {  # 🕐
         'en': ':one_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock1:'],
+        'alias': [':clock1:', ':one_oclock:'],
         'variant': True,
         'de': ':1.00_uhr:',
         'es': ':1_en_punto:',
         'fr': ':une_heure:',
         'ja': ':1時:',
         'ko': ':한_시:',
         'pt': ':1_hora:',
@@ -41541,35 +42092,85 @@
         'fa': ':کف_دست_به_پایین:',
         'id': ':telapak_tangan_menghadap_ke_bawah:',
         'zh': ':掌心向下的手:'
     },
     '\U0001FAF3\U0001F3FF': {  # 🫳🏿
         'en': ':palm_down_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_unten_dunkle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_abajo_tono_de_piel_oscuro:',
+        'fr': ':main_paume_vers_le_bas__peau_foncée:',
+        'ja': ':下に向けた手_濃い肌色:',
+        'ko': ':손바닥을_아래로_향한_손_검은색_피부:',
+        'pt': ':mão_com_a_palma_para_baixo_pele_escura:',
+        'it': ':mano_con_il_palmo_verso_il_basso_carnagione_scura:',
+        'fa': ':کف_دست_به_پایین_پوست_آبنوسی:',
+        'id': ':telapak_tangan_menghadap_ke_bawah_warna_kulit_gelap:',
+        'zh': ':掌心向下的手_较深肤色:'
     },
     '\U0001FAF3\U0001F3FB': {  # 🫳🏻
         'en': ':palm_down_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_unten_helle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_abajo_tono_de_piel_claro:',
+        'fr': ':main_paume_vers_le_bas__peau_claire:',
+        'ja': ':下に向けた手_薄い肌色:',
+        'ko': ':손바닥을_아래로_향한_손_하얀_피부:',
+        'pt': ':mão_com_a_palma_para_baixo_pele_clara:',
+        'it': ':mano_con_il_palmo_verso_il_basso_carnagione_chiara:',
+        'fa': ':کف_دست_به_پایین_پوست_سفید:',
+        'id': ':telapak_tangan_menghadap_ke_bawah_warna_kulit_cerah:',
+        'zh': ':掌心向下的手_较浅肤色:'
     },
     '\U0001FAF3\U0001F3FE': {  # 🫳🏾
         'en': ':palm_down_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_unten_mitteldunkle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_abajo_tono_de_piel_oscuro_medio:',
+        'fr': ':main_paume_vers_le_bas__peau_mate:',
+        'ja': ':下に向けた手_やや濃い肌色:',
+        'ko': ':손바닥을_아래로_향한_손_진한_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_baixo_pele_morena_escura:',
+        'it': ':mano_con_il_palmo_verso_il_basso_carnagione_abbastanza_scura:',
+        'fa': ':کف_دست_به_پایین_پوست_گندمی:',
+        'id': ':telapak_tangan_menghadap_ke_bawah_warna_kulit_gelap-sedang:',
+        'zh': ':掌心向下的手_中等深肤色:'
     },
     '\U0001FAF3\U0001F3FC': {  # 🫳🏼
         'en': ':palm_down_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_unten_mittelhelle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_abajo_tono_de_piel_claro_medio:',
+        'fr': ':main_paume_vers_le_bas__peau_moyennement_claire:',
+        'ja': ':下に向けた手_やや薄い肌色:',
+        'ko': ':손바닥을_아래로_향한_손_연한_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_baixo_pele_morena_clara:',
+        'it': ':mano_con_il_palmo_verso_il_basso_carnagione_abbastanza_chiara:',
+        'fa': ':کف_دست_به_پایین_پوست_روشن:',
+        'id': ':telapak_tangan_menghadap_ke_bawah_warna_kulit_cerah-sedang:',
+        'zh': ':掌心向下的手_中等浅肤色:'
     },
     '\U0001FAF3\U0001F3FD': {  # 🫳🏽
         'en': ':palm_down_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_unten_mittlere_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_abajo_tono_de_piel_medio:',
+        'fr': ':main_paume_vers_le_bas__peau_légèrement_mate:',
+        'ja': ':下に向けた手_中間の肌色:',
+        'ko': ':손바닥을_아래로_향한_손_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_baixo_pele_morena:',
+        'it': ':mano_con_il_palmo_verso_il_basso_carnagione_olivastra:',
+        'fa': ':کف_دست_به_پایین_پوست_طلایی:',
+        'id': ':telapak_tangan_menghadap_ke_bawah_warna_kulit_sedang:',
+        'zh': ':掌心向下的手_中等肤色:'
     },
     '\U0001F334': {  # 🌴
         'en': ':palm_tree:',
         'status': fully_qualified,
         'E': 0.6,
         'de': ':palme:',
         'es': ':palmera:',
@@ -41596,35 +42197,85 @@
         'fa': ':کف_دست_به_بالا:',
         'id': ':telapak_tangan_menghadap_ke_atas:',
         'zh': ':掌心向上的手:'
     },
     '\U0001FAF4\U0001F3FF': {  # 🫴🏿
         'en': ':palm_up_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_oben_dunkle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_arriba_tono_de_piel_oscuro:',
+        'fr': ':main_paume_vers_le_haut__peau_foncée:',
+        'ja': ':上に向けた手_濃い肌色:',
+        'ko': ':손바닥을_위로_향한_손_검은색_피부:',
+        'pt': ':mão_com_a_palma_para_cima_pele_escura:',
+        'it': ':mano_con_il_palmo_verso_l’alto_carnagione_scura:',
+        'fa': ':کف_دست_به_بالا_پوست_آبنوسی:',
+        'id': ':telapak_tangan_menghadap_ke_atas_warna_kulit_gelap:',
+        'zh': ':掌心向上的手_较深肤色:'
     },
     '\U0001FAF4\U0001F3FB': {  # 🫴🏻
         'en': ':palm_up_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_oben_helle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_arriba_tono_de_piel_claro:',
+        'fr': ':main_paume_vers_le_haut__peau_claire:',
+        'ja': ':上に向けた手_薄い肌色:',
+        'ko': ':손바닥을_위로_향한_손_하얀_피부:',
+        'pt': ':mão_com_a_palma_para_cima_pele_clara:',
+        'it': ':mano_con_il_palmo_verso_l’alto_carnagione_chiara:',
+        'fa': ':کف_دست_به_بالا_پوست_سفید:',
+        'id': ':telapak_tangan_menghadap_ke_atas_warna_kulit_cerah:',
+        'zh': ':掌心向上的手_较浅肤色:'
     },
     '\U0001FAF4\U0001F3FE': {  # 🫴🏾
         'en': ':palm_up_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_oben_mitteldunkle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_arriba_tono_de_piel_oscuro_medio:',
+        'fr': ':main_paume_vers_le_haut__peau_mate:',
+        'ja': ':上に向けた手_やや濃い肌色:',
+        'ko': ':손바닥을_위로_향한_손_진한_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_cima_pele_morena_escura:',
+        'it': ':mano_con_il_palmo_verso_l’alto_carnagione_abbastanza_scura:',
+        'fa': ':کف_دست_به_بالا_پوست_گندمی:',
+        'id': ':telapak_tangan_menghadap_ke_atas_warna_kulit_gelap-sedang:',
+        'zh': ':掌心向上的手_中等深肤色:'
     },
     '\U0001FAF4\U0001F3FC': {  # 🫴🏼
         'en': ':palm_up_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_oben_mittelhelle_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_arriba_tono_de_piel_claro_medio:',
+        'fr': ':main_paume_vers_le_haut__peau_moyennement_claire:',
+        'ja': ':上に向けた手_やや薄い肌色:',
+        'ko': ':손바닥을_위로_향한_손_연한_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_cima_pele_morena_clara:',
+        'it': ':mano_con_il_palmo_verso_l’alto_carnagione_abbastanza_chiara:',
+        'fa': ':کف_دست_به_بالا_پوست_روشن:',
+        'id': ':telapak_tangan_menghadap_ke_atas_warna_kulit_cerah-sedang:',
+        'zh': ':掌心向上的手_中等浅肤色:'
     },
     '\U0001FAF4\U0001F3FD': {  # 🫴🏽
         'en': ':palm_up_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':hand_mit_handfläche_nach_oben_mittlere_hautfarbe:',
+        'es': ':mano_con_la_palma_hacia_arriba_tono_de_piel_medio:',
+        'fr': ':main_paume_vers_le_haut__peau_légèrement_mate:',
+        'ja': ':上に向けた手_中間の肌色:',
+        'ko': ':손바닥을_위로_향한_손_갈색_피부:',
+        'pt': ':mão_com_a_palma_para_cima_pele_morena:',
+        'it': ':mano_con_il_palmo_verso_l’alto_carnagione_olivastra:',
+        'fa': ':کف_دست_به_بالا_پوست_طلایی:',
+        'id': ':telapak_tangan_menghadap_ke_atas_warna_kulit_sedang:',
+        'zh': ':掌心向上的手_中等肤色:'
     },
     '\U0001F932': {  # 🤲
         'en': ':palms_up_together:',
         'status': fully_qualified,
         'E': 5,
         'de': ':handflächen_nach_oben:',
         'es': ':palmas_hacia_arriba_juntas:',
@@ -43566,15 +44217,15 @@
         'id': ':orang_marah_warna_kulit_sedang:',
         'zh': ':皱眉_中等肤色:'
     },
     '\U0001F645': {  # 🙅
         'en': ':person_gesturing_NO:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':no_good:'],
+        'alias': [':no_good:', ':person_gesturing_no:'],
         'de': ':person_mit_überkreuzten_armen:',
         'es': ':persona_haciendo_el_gesto_de_no:',
         'fr': ':personne_faisant_un_geste_d’interdiction:',
         'ja': ':ダメのポーズをする人:',
         'ko': ':안_된다는_제스처를_하는_사람:',
         'pt': ':pessoa_fazendo_gesto_de_“não”:',
         'it': ':persona_che_fa_segno_di_no:',
@@ -43657,15 +44308,15 @@
         'id': ':orang_mengisyaratkan_tidak_warna_kulit_sedang:',
         'zh': ':禁止手势_中等肤色:'
     },
     '\U0001F646': {  # 🙆
         'en': ':person_gesturing_OK:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':ok_person:'],
+        'alias': [':ok_person:', ':person_gesturing_ok:'],
         'de': ':person_mit_händen_auf_dem_kopf:',
         'es': ':persona_haciendo_el_gesto_de_de_acuerdo:',
         'fr': ':personne_faisant_un_geste_d’acceptation:',
         'ja': ':okのポーズをする人:',
         'ko': ':오케이라는_제스처를_하는_사람:',
         'pt': ':pessoa_fazendo_gesto_de_“ok”:',
         'it': ':persona_con_gesto_ok:',
@@ -46813,35 +47464,85 @@
         'fa': ':آدم_تاج_دار:',
         'id': ':orang_mengenakan_mahkota:',
         'zh': ':戴王冠的人:'
     },
     '\U0001FAC5\U0001F3FF': {  # 🫅🏿
         'en': ':person_with_crown_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':person_mit_krone_dunkle_hautfarbe:',
+        'es': ':persona_con_corona_tono_de_piel_oscuro:',
+        'fr': ':personne_avec_une_couronne__peau_foncée:',
+        'ja': ':王冠をかぶった人_濃い肌色:',
+        'ko': ':왕관을_쓴_사람_검은색_피부:',
+        'pt': ':pessoa_com_coroa_pele_escura:',
+        'it': ':persona_con_corona_carnagione_scura:',
+        'fa': ':آدم_تاج_دار_پوست_آبنوسی:',
+        'id': ':orang_mengenakan_mahkota_warna_kulit_gelap:',
+        'zh': ':戴王冠的人_较深肤色:'
     },
     '\U0001FAC5\U0001F3FB': {  # 🫅🏻
         'en': ':person_with_crown_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':person_mit_krone_helle_hautfarbe:',
+        'es': ':persona_con_corona_tono_de_piel_claro:',
+        'fr': ':personne_avec_une_couronne__peau_claire:',
+        'ja': ':王冠をかぶった人_薄い肌色:',
+        'ko': ':왕관을_쓴_사람_하얀_피부:',
+        'pt': ':pessoa_com_coroa_pele_clara:',
+        'it': ':persona_con_corona_carnagione_chiara:',
+        'fa': ':آدم_تاج_دار_پوست_سفید:',
+        'id': ':orang_mengenakan_mahkota_warna_kulit_cerah:',
+        'zh': ':戴王冠的人_较浅肤色:'
     },
     '\U0001FAC5\U0001F3FE': {  # 🫅🏾
         'en': ':person_with_crown_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':person_mit_krone_mitteldunkle_hautfarbe:',
+        'es': ':persona_con_corona_tono_de_piel_oscuro_medio:',
+        'fr': ':personne_avec_une_couronne__peau_mate:',
+        'ja': ':王冠をかぶった人_やや濃い肌色:',
+        'ko': ':왕관을_쓴_사람_진한_갈색_피부:',
+        'pt': ':pessoa_com_coroa_pele_morena_escura:',
+        'it': ':persona_con_corona_carnagione_abbastanza_scura:',
+        'fa': ':آدم_تاج_دار_پوست_گندمی:',
+        'id': ':orang_mengenakan_mahkota_warna_kulit_gelap-sedang:',
+        'zh': ':戴王冠的人_中等深肤色:'
     },
     '\U0001FAC5\U0001F3FC': {  # 🫅🏼
         'en': ':person_with_crown_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':person_mit_krone_mittelhelle_hautfarbe:',
+        'es': ':persona_con_corona_tono_de_piel_claro_medio:',
+        'fr': ':personne_avec_une_couronne__peau_moyennement_claire:',
+        'ja': ':王冠をかぶった人_やや薄い肌色:',
+        'ko': ':왕관을_쓴_사람_연한_갈색_피부:',
+        'pt': ':pessoa_com_coroa_pele_morena_clara:',
+        'it': ':persona_con_corona_carnagione_abbastanza_chiara:',
+        'fa': ':آدم_تاج_دار_پوست_روشن:',
+        'id': ':orang_mengenakan_mahkota_warna_kulit_cerah-sedang:',
+        'zh': ':戴王冠的人_中等浅肤色:'
     },
     '\U0001FAC5\U0001F3FD': {  # 🫅🏽
         'en': ':person_with_crown_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':person_mit_krone_mittlere_hautfarbe:',
+        'es': ':persona_con_corona_tono_de_piel_medio:',
+        'fr': ':personne_avec_une_couronne__peau_légèrement_mate:',
+        'ja': ':王冠をかぶった人_中間の肌色:',
+        'ko': ':왕관을_쓴_사람_갈색_피부:',
+        'pt': ':pessoa_com_coroa_pele_morena:',
+        'it': ':persona_con_corona_carnagione_olivastra:',
+        'fa': ':آدم_تاج_دار_پوست_طلایی:',
+        'id': ':orang_mengenakan_mahkota_warna_kulit_sedang:',
+        'zh': ':戴王冠的人_中等肤色:'
     },
     '\U0001F472': {  # 👲
         'en': ':person_with_skullcap:',
         'status': fully_qualified,
         'E': 0.6,
         'alias': [':man_with_gua_pi_mao:'],
         'de': ':mann_mit_chinesischem_hut:',
@@ -47813,15 +48514,15 @@
         'id': ':tombol_putar:',
         'zh': ':播放按钮:'
     },
     '\U000023EF\U0000FE0F': {  # ⏯️
         'en': ':play_or_pause_button:',
         'status': fully_qualified,
         'E': 1,
-        'alias': [':black_right__pointing_triangle_with_double_vertical_bar:'],
+        'alias': [':black_right__pointing_triangle_with_double_vertical_bar:', ':black_right_pointing_triangle_with_double_vertical_bar:'],
         'variant': True,
         'de': ':wiedergabe_oder_pause:',
         'es': ':reproducir_o_pausa:',
         'fr': ':bouton_lecture/pause:',
         'ja': ':再生/一時停止ボタン:',
         'ko': ':재생_또는_일시_정지_버튼:',
         'pt': ':botão_de_reproduzir_ou_pausar:',
@@ -47830,15 +48531,15 @@
         'id': ':tombol_putar_atau_jeda:',
         'zh': ':播放或暂停按钮:'
     },
     '\U000023EF': {  # ⏯
         'en': ':play_or_pause_button:',
         'status': unqualified,
         'E': 1,
-        'alias': [':black_right__pointing_triangle_with_double_vertical_bar:'],
+        'alias': [':black_right__pointing_triangle_with_double_vertical_bar:', ':black_right_pointing_triangle_with_double_vertical_bar:'],
         'variant': True,
         'de': ':wiedergabe_oder_pause:',
         'es': ':reproducir_o_pausa:',
         'fr': ':bouton_lecture/pause:',
         'ja': ':再生/一時停止ボタン:',
         'ko': ':재생_또는_일시_정지_버튼:',
         'pt': ':botão_de_reproduzir_ou_pausar:',
@@ -48303,35 +49004,85 @@
         'fa': ':مرد_باردار:',
         'id': ':pria_hamil:',
         'zh': ':怀孕的男人:'
     },
     '\U0001FAC3\U0001F3FF': {  # 🫃🏿
         'en': ':pregnant_man_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangerer_mann_dunkle_hautfarbe:',
+        'es': ':hombre_embarazado_tono_de_piel_oscuro:',
+        'fr': ':homme_enceint__peau_foncée:',
+        'ja': ':妊夫_濃い肌色:',
+        'ko': ':임신한_남자_검은색_피부:',
+        'pt': ':homem_grávido_pele_escura:',
+        'it': ':uomo_incinto_carnagione_scura:',
+        'fa': ':مرد_باردار_پوست_آبنوسی:',
+        'id': ':pria_hamil_warna_kulit_gelap:',
+        'zh': ':怀孕的男人_较深肤色:'
     },
     '\U0001FAC3\U0001F3FB': {  # 🫃🏻
         'en': ':pregnant_man_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangerer_mann_helle_hautfarbe:',
+        'es': ':hombre_embarazado_tono_de_piel_claro:',
+        'fr': ':homme_enceint__peau_claire:',
+        'ja': ':妊夫_薄い肌色:',
+        'ko': ':임신한_남자_하얀_피부:',
+        'pt': ':homem_grávido_pele_clara:',
+        'it': ':uomo_incinto_carnagione_chiara:',
+        'fa': ':مرد_باردار_پوست_سفید:',
+        'id': ':pria_hamil_warna_kulit_cerah:',
+        'zh': ':怀孕的男人_较浅肤色:'
     },
     '\U0001FAC3\U0001F3FE': {  # 🫃🏾
         'en': ':pregnant_man_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangerer_mann_mitteldunkle_hautfarbe:',
+        'es': ':hombre_embarazado_tono_de_piel_oscuro_medio:',
+        'fr': ':homme_enceint__peau_mate:',
+        'ja': ':妊夫_やや濃い肌色:',
+        'ko': ':임신한_남자_진한_갈색_피부:',
+        'pt': ':homem_grávido_pele_morena_escura:',
+        'it': ':uomo_incinto_carnagione_abbastanza_scura:',
+        'fa': ':مرد_باردار_پوست_گندمی:',
+        'id': ':pria_hamil_warna_kulit_gelap-sedang:',
+        'zh': ':怀孕的男人_中等深肤色:'
     },
     '\U0001FAC3\U0001F3FC': {  # 🫃🏼
         'en': ':pregnant_man_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangerer_mann_mittelhelle_hautfarbe:',
+        'es': ':hombre_embarazado_tono_de_piel_claro_medio:',
+        'fr': ':homme_enceint__peau_moyennement_claire:',
+        'ja': ':妊夫_やや薄い肌色:',
+        'ko': ':임신한_남자_연한_갈색_피부:',
+        'pt': ':homem_grávido_pele_morena_clara:',
+        'it': ':uomo_incinto_carnagione_abbastanza_chiara:',
+        'fa': ':مرد_باردار_پوست_روشن:',
+        'id': ':pria_hamil_warna_kulit_cerah-sedang:',
+        'zh': ':怀孕的男人_中等浅肤色:'
     },
     '\U0001FAC3\U0001F3FD': {  # 🫃🏽
         'en': ':pregnant_man_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangerer_mann_mittlere_hautfarbe:',
+        'es': ':hombre_embarazado_tono_de_piel_medio:',
+        'fr': ':homme_enceint__peau_légèrement_mate:',
+        'ja': ':妊夫_中間の肌色:',
+        'ko': ':임신한_남자_갈색_피부:',
+        'pt': ':homem_grávido_pele_morena:',
+        'it': ':uomo_incinto_carnagione_olivastra:',
+        'fa': ':مرد_باردار_پوست_طلایی:',
+        'id': ':pria_hamil_warna_kulit_sedang:',
+        'zh': ':怀孕的男人_中等肤色:'
     },
     '\U0001FAC4': {  # 🫄
         'en': ':pregnant_person:',
         'status': fully_qualified,
         'E': 14,
         'de': ':schwangere_person:',
         'es': ':persona_embarazada:',
@@ -48343,35 +49094,85 @@
         'fa': ':آدم_باردار:',
         'id': ':orang_hamil:',
         'zh': ':怀孕的人:'
     },
     '\U0001FAC4\U0001F3FF': {  # 🫄🏿
         'en': ':pregnant_person_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangere_person_dunkle_hautfarbe:',
+        'es': ':persona_embarazada_tono_de_piel_oscuro:',
+        'fr': ':personne_enceinte__peau_foncée:',
+        'ja': ':妊娠した人_濃い肌色:',
+        'ko': ':임신한_사람_검은색_피부:',
+        'pt': ':pessoa_grávida_pele_escura:',
+        'it': ':persona_incinta_carnagione_scura:',
+        'fa': ':آدم_باردار_پوست_آبنوسی:',
+        'id': ':orang_hamil_warna_kulit_gelap:',
+        'zh': ':怀孕的人_较深肤色:'
     },
     '\U0001FAC4\U0001F3FB': {  # 🫄🏻
         'en': ':pregnant_person_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangere_person_helle_hautfarbe:',
+        'es': ':persona_embarazada_tono_de_piel_claro:',
+        'fr': ':personne_enceinte__peau_claire:',
+        'ja': ':妊娠した人_薄い肌色:',
+        'ko': ':임신한_사람_하얀_피부:',
+        'pt': ':pessoa_grávida_pele_clara:',
+        'it': ':persona_incinta_carnagione_chiara:',
+        'fa': ':آدم_باردار_پوست_سفید:',
+        'id': ':orang_hamil_warna_kulit_cerah:',
+        'zh': ':怀孕的人_较浅肤色:'
     },
     '\U0001FAC4\U0001F3FE': {  # 🫄🏾
         'en': ':pregnant_person_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangere_person_mitteldunkle_hautfarbe:',
+        'es': ':persona_embarazada_tono_de_piel_oscuro_medio:',
+        'fr': ':personne_enceinte__peau_mate:',
+        'ja': ':妊娠した人_やや濃い肌色:',
+        'ko': ':임신한_사람_진한_갈색_피부:',
+        'pt': ':pessoa_grávida_pele_morena_escura:',
+        'it': ':persona_incinta_carnagione_abbastanza_scura:',
+        'fa': ':آدم_باردار_پوست_گندمی:',
+        'id': ':orang_hamil_warna_kulit_gelap-sedang:',
+        'zh': ':怀孕的人_中等深肤色:'
     },
     '\U0001FAC4\U0001F3FC': {  # 🫄🏼
         'en': ':pregnant_person_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangere_person_mittelhelle_hautfarbe:',
+        'es': ':persona_embarazada_tono_de_piel_claro_medio:',
+        'fr': ':personne_enceinte__peau_moyennement_claire:',
+        'ja': ':妊娠した人_やや薄い肌色:',
+        'ko': ':임신한_사람_연한_갈색_피부:',
+        'pt': ':pessoa_grávida_pele_morena_clara:',
+        'it': ':persona_incinta_carnagione_abbastanza_chiara:',
+        'fa': ':آدم_باردار_پوست_روشن:',
+        'id': ':orang_hamil_warna_kulit_cerah-sedang:',
+        'zh': ':怀孕的人_中等浅肤色:'
     },
     '\U0001FAC4\U0001F3FD': {  # 🫄🏽
         'en': ':pregnant_person_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':schwangere_person_mittlere_hautfarbe:',
+        'es': ':persona_embarazada_tono_de_piel_medio:',
+        'fr': ':personne_enceinte__peau_légèrement_mate:',
+        'ja': ':妊娠した人_中間の肌色:',
+        'ko': ':임신한_사람_갈색_피부:',
+        'pt': ':pessoa_grávida_pele_morena:',
+        'it': ':persona_incinta_carnagione_olivastra:',
+        'fa': ':آدم_باردار_پوست_طلایی:',
+        'id': ':orang_hamil_warna_kulit_sedang:',
+        'zh': ':怀孕的人_中等肤色:'
     },
     '\U0001F930': {  # 🤰
         'en': ':pregnant_woman:',
         'status': fully_qualified,
         'E': 3,
         'de': ':schwangere_frau:',
         'es': ':mujer_embarazada:',
@@ -49824,15 +50625,15 @@
         'id': ':tombol_ulangi_satu_lagu:',
         'zh': ':重复一次按钮:'
     },
     '\U000026D1\U0000FE0F': {  # ⛑️
         'en': ':rescue_worker’s_helmet:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':helmet_with_white_cross:', ':rescue_worker_helmet:'],
+        'alias': [':helmet_with_white_cross:', ':rescue_worker_helmet:', ':rescue_workers_helmet:'],
         'variant': True,
         'de': ':rettungshelm:',
         'es': ':casco_con_una_cruz_blanca:',
         'fr': ':casque_de_secouriste:',
         'ja': ':白十字ヘルメット:',
         'ko': ':흰_십자가가_있는_헬멧:',
         'pt': ':capacacete_de_socorrista:',
@@ -49841,15 +50642,15 @@
         'id': ':helm_dengan_palang_putih:',
         'zh': ':白十字头盔:'
     },
     '\U000026D1': {  # ⛑
         'en': ':rescue_worker’s_helmet:',
         'status': unqualified,
         'E': 0.7,
-        'alias': [':helmet_with_white_cross:', ':rescue_worker_helmet:'],
+        'alias': [':helmet_with_white_cross:', ':rescue_worker_helmet:', ':rescue_workers_helmet:'],
         'variant': True,
         'de': ':rettungshelm:',
         'es': ':casco_con_una_cruz_blanca:',
         'fr': ':casque_de_secouriste:',
         'ja': ':白十字ヘルメット:',
         'ko': ':흰_십자가가_있는_헬멧:',
         'pt': ':capacacete_de_socorrista:',
@@ -49982,15 +50783,15 @@
         'id': ':kerupuk_beras:',
         'zh': ':米饼:'
     },
     '\U0001F91C': {  # 🤜
         'en': ':right-facing_fist:',
         'status': fully_qualified,
         'E': 3,
-        'alias': [':fist_right:'],
+        'alias': [':fist_right:', ':right_facing_fist:'],
         'de': ':faust_nach_rechts:',
         'es': ':puño_hacia_la_derecha:',
         'fr': ':poing_à_droite:',
         'ja': ':右向きのこぶし:',
         'ko': ':오른쪽을_향하는_주먹:',
         'pt': ':punho_direito:',
         'it': ':pugno_a_destra:',
@@ -50255,35 +51056,85 @@
         'fa': ':دست_به_سمت_راست:',
         'id': ':tangan_menghadap_kanan:',
         'zh': ':向右的手:'
     },
     '\U0001FAF1\U0001F3FF': {  # 🫱🏿
         'en': ':rightwards_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_rechts_weisende_hand_dunkle_hautfarbe:',
+        'es': ':mano_hacia_la_derecha_tono_de_piel_oscuro:',
+        'fr': ':main_vers_la_droite__peau_foncée:',
+        'ja': ':右に向けた手_濃い肌色:',
+        'ko': ':오른쪽으로_향하는_손등_검은색_피부:',
+        'pt': ':mão_para_a_direita_pele_escura:',
+        'it': ':mano_rivolta_a_destra_carnagione_scura:',
+        'fa': ':دست_به_سمت_راست_پوست_آبنوسی:',
+        'id': ':tangan_menghadap_kanan_warna_kulit_gelap:',
+        'zh': ':向右的手_较深肤色:'
     },
     '\U0001FAF1\U0001F3FB': {  # 🫱🏻
         'en': ':rightwards_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_rechts_weisende_hand_helle_hautfarbe:',
+        'es': ':mano_hacia_la_derecha_tono_de_piel_claro:',
+        'fr': ':main_vers_la_droite__peau_claire:',
+        'ja': ':右に向けた手_薄い肌色:',
+        'ko': ':오른쪽으로_향하는_손등_하얀_피부:',
+        'pt': ':mão_para_a_direita_pele_clara:',
+        'it': ':mano_rivolta_a_destra_carnagione_chiara:',
+        'fa': ':دست_به_سمت_راست_پوست_سفید:',
+        'id': ':tangan_menghadap_kanan_warna_kulit_cerah:',
+        'zh': ':向右的手_较浅肤色:'
     },
     '\U0001FAF1\U0001F3FE': {  # 🫱🏾
         'en': ':rightwards_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_rechts_weisende_hand_mitteldunkle_hautfarbe:',
+        'es': ':mano_hacia_la_derecha_tono_de_piel_oscuro_medio:',
+        'fr': ':main_vers_la_droite__peau_mate:',
+        'ja': ':右に向けた手_やや濃い肌色:',
+        'ko': ':오른쪽으로_향하는_손등_진한_갈색_피부:',
+        'pt': ':mão_para_a_direita_pele_morena_escura:',
+        'it': ':mano_rivolta_a_destra_carnagione_abbastanza_scura:',
+        'fa': ':دست_به_سمت_راست_پوست_گندمی:',
+        'id': ':tangan_menghadap_kanan_warna_kulit_gelap-sedang:',
+        'zh': ':向右的手_中等深肤色:'
     },
     '\U0001FAF1\U0001F3FC': {  # 🫱🏼
         'en': ':rightwards_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_rechts_weisende_hand_mittelhelle_hautfarbe:',
+        'es': ':mano_hacia_la_derecha_tono_de_piel_claro_medio:',
+        'fr': ':main_vers_la_droite__peau_moyennement_claire:',
+        'ja': ':右に向けた手_やや薄い肌色:',
+        'ko': ':오른쪽으로_향하는_손등_연한_갈색_피부:',
+        'pt': ':mão_para_a_direita_pele_morena_clara:',
+        'it': ':mano_rivolta_a_destra_carnagione_abbastanza_chiara:',
+        'fa': ':دست_به_سمت_راست_پوست_روشن:',
+        'id': ':tangan_menghadap_kanan_warna_kulit_cerah-sedang:',
+        'zh': ':向右的手_中等浅肤色:'
     },
     '\U0001FAF1\U0001F3FD': {  # 🫱🏽
         'en': ':rightwards_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 14
+        'E': 14,
+        'de': ':nach_rechts_weisende_hand_mittlere_hautfarbe:',
+        'es': ':mano_hacia_la_derecha_tono_de_piel_medio:',
+        'fr': ':main_vers_la_droite__peau_légèrement_mate:',
+        'ja': ':右に向けた手_中間の肌色:',
+        'ko': ':오른쪽으로_향하는_손등_갈색_피부:',
+        'pt': ':mão_para_a_direita_pele_morena:',
+        'it': ':mano_rivolta_a_destra_carnagione_olivastra:',
+        'fa': ':دست_به_سمت_راست_پوست_طلایی:',
+        'id': ':tangan_menghadap_kanan_warna_kulit_sedang:',
+        'zh': ':向右的手_中等肤色:'
     },
     '\U0001FAF8': {  # 🫸
         'en': ':rightwards_pushing_hand:',
         'status': fully_qualified,
         'E': 15,
         'de': ':nach_rechts_schiebende_hand:',
         'es': ':mano_empujando_hacia_la_derecha:',
@@ -50295,35 +51146,85 @@
         'fa': ':دست_فشاردهنده_به_سمت_راست:',
         'id': ':tangan_mendorong_ke_kanan:',
         'zh': ':向右推:'
     },
     '\U0001FAF8\U0001F3FF': {  # 🫸🏿
         'en': ':rightwards_pushing_hand_dark_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_rechts_schiebende_hand_dunkle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_derecha_tono_de_piel_oscuro:',
+        'fr': ':main_qui_pousse_vers_la_droite__peau_foncée:',
+        'ja': ':右向きに押している手_濃い肌色:',
+        'ko': ':오른쪽으로_밀치는_손_검은색_피부:',
+        'pt': ':mão_empurrando_para_a_direita_pele_escura:',
+        'it': ':mano_che_spinge_a_destra_carnagione_scura:',
+        'fa': ':دست_فشاردهنده_به_سمت_راست_پوست_آبنوسی:',
+        'id': ':tangan_mendorong_ke_kanan_warna_kulit_gelap:',
+        'zh': ':向右推_较深肤色:'
     },
     '\U0001FAF8\U0001F3FB': {  # 🫸🏻
         'en': ':rightwards_pushing_hand_light_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_rechts_schiebende_hand_helle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_derecha_tono_de_piel_claro:',
+        'fr': ':main_qui_pousse_vers_la_droite__peau_claire:',
+        'ja': ':右向きに押している手_薄い肌色:',
+        'ko': ':오른쪽으로_밀치는_손_하얀_피부:',
+        'pt': ':mão_empurrando_para_a_direita_pele_clara:',
+        'it': ':mano_che_spinge_a_destra_carnagione_chiara:',
+        'fa': ':دست_فشاردهنده_به_سمت_راست_پوست_سفید:',
+        'id': ':tangan_mendorong_ke_kanan_warna_kulit_cerah:',
+        'zh': ':向右推_较浅肤色:'
     },
     '\U0001FAF8\U0001F3FE': {  # 🫸🏾
         'en': ':rightwards_pushing_hand_medium-dark_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_rechts_schiebende_hand_mitteldunkle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_derecha_tono_de_piel_oscuro_medio:',
+        'fr': ':main_qui_pousse_vers_la_droite__peau_mate:',
+        'ja': ':右向きに押している手_やや濃い肌色:',
+        'ko': ':오른쪽으로_밀치는_손_진한_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_direita_pele_morena_escura:',
+        'it': ':mano_che_spinge_a_destra_carnagione_abbastanza_scura:',
+        'fa': ':دست_فشاردهنده_به_سمت_راست_پوست_گندمی:',
+        'id': ':tangan_mendorong_ke_kanan_warna_kulit_gelap-sedang:',
+        'zh': ':向右推_中等深肤色:'
     },
     '\U0001FAF8\U0001F3FC': {  # 🫸🏼
         'en': ':rightwards_pushing_hand_medium-light_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_rechts_schiebende_hand_mittelhelle_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_derecha_tono_de_piel_claro_medio:',
+        'fr': ':main_qui_pousse_vers_la_droite__peau_moyennement_claire:',
+        'ja': ':右向きに押している手_やや薄い肌色:',
+        'ko': ':오른쪽으로_밀치는_손_연한_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_direita_pele_morena_clara:',
+        'it': ':mano_che_spinge_a_destra_carnagione_abbastanza_chiara:',
+        'fa': ':دست_فشاردهنده_به_سمت_راست_پوست_روشن:',
+        'id': ':tangan_mendorong_ke_kanan_warna_kulit_cerah-sedang:',
+        'zh': ':向右推_中等浅肤色:'
     },
     '\U0001FAF8\U0001F3FD': {  # 🫸🏽
         'en': ':rightwards_pushing_hand_medium_skin_tone:',
         'status': fully_qualified,
-        'E': 15
+        'E': 15,
+        'de': ':nach_rechts_schiebende_hand_mittlere_hautfarbe:',
+        'es': ':mano_empujando_hacia_la_derecha_tono_de_piel_medio:',
+        'fr': ':main_qui_pousse_vers_la_droite__peau_légèrement_mate:',
+        'ja': ':右向きに押している手_中間の肌色:',
+        'ko': ':오른쪽으로_밀치는_손_갈색_피부:',
+        'pt': ':mão_empurrando_para_a_direita_pele_morena:',
+        'it': ':mano_che_spinge_a_destra_carnagione_olivastra:',
+        'fa': ':دست_فشاردهنده_به_سمت_راست_پوست_طلایی:',
+        'id': ':tangan_mendorong_ke_kanan_warna_kulit_sedang:',
+        'zh': ':向右推_中等肤色:'
     },
     '\U0001F48D': {  # 💍
         'en': ':ring:',
         'status': fully_qualified,
         'E': 0.6,
         'de': ':ring:',
         'es': ':anillo:',
@@ -50443,15 +51344,15 @@
         'id': ':gulungan_kertas:',
         'zh': ':卷纸:'
     },
     '\U0001F5DE\U0000FE0F': {  # 🗞️
         'en': ':rolled-up_newspaper:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':rolled__up_newspaper:', ':newspaper_roll:'],
+        'alias': [':rolled__up_newspaper:', ':newspaper_roll:', ':rolled_up_newspaper:'],
         'variant': True,
         'de': ':zusammengerollte_zeitung:',
         'es': ':periódico_enrollado:',
         'fr': ':journal_roulé:',
         'ja': ':丸めた新聞:',
         'ko': ':돌돌_말린_신문:',
         'pt': ':jornal_enrolado:',
@@ -50460,15 +51361,15 @@
         'id': ':gulungan_koran:',
         'zh': ':报纸卷:'
     },
     '\U0001F5DE': {  # 🗞
         'en': ':rolled-up_newspaper:',
         'status': unqualified,
         'E': 0.7,
-        'alias': [':rolled__up_newspaper:', ':newspaper_roll:'],
+        'alias': [':rolled__up_newspaper:', ':newspaper_roll:', ':rolled_up_newspaper:'],
         'variant': True,
         'de': ':zusammengerollte_zeitung:',
         'es': ':periódico_enrollado:',
         'fr': ':journal_roulé:',
         'ja': ':丸めた新聞:',
         'ko': ':돌돌_말린_신문:',
         'pt': ':jornal_enrolado:',
@@ -51092,15 +51993,15 @@
         'id': ':kursi:',
         'zh': ':座位:'
     },
     '\U0001F648': {  # 🙈
         'en': ':see-no-evil_monkey:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':see_no_evil:'],
+        'alias': [':see_no_evil:', ':see_no_evil_monkey:'],
         'de': ':sich_die_augen_zuhaltendes_affengesicht:',
         'es': ':mono_con_los_ojos_tapados:',
         'fr': ':singe_ne_rien_voir:',
         'ja': ':見ざる:',
         'ko': ':눈을_가리고_있는_원숭이:',
         'pt': ':macaco_que_não_vê_nada:',
         'it': ':non_vedo:',
@@ -51228,15 +52129,15 @@
         'id': ':anjing_pembimbing:',
         'zh': ':服务犬:'
     },
     '\U0001F562': {  # 🕢
         'en': ':seven-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock730:'],
+        'alias': [':clock730:', ':seven_thirty:'],
         'variant': True,
         'de': ':7.30_uhr:',
         'es': ':siete_y_media:',
         'fr': ':sept_heures_et_demie:',
         'ja': ':7時半:',
         'ko': ':일곱_시_반:',
         'pt': ':sete_e_meia:',
@@ -51245,15 +52146,15 @@
         'id': ':jam_setengah_delapan:',
         'zh': ':七点半:'
     },
     '\U0001F556': {  # 🕖
         'en': ':seven_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock7:'],
+        'alias': [':clock7:', ':seven_oclock:'],
         'variant': True,
         'de': ':7.00_uhr:',
         'es': ':7_en_punto:',
         'fr': ':sept_heures:',
         'ja': ':7時:',
         'ko': ':일곱_시:',
         'pt': ':7_horas:',
@@ -51802,15 +52703,15 @@
         'id': ':penyanyi_warna_kulit_sedang:',
         'zh': ':歌手_中等肤色:'
     },
     '\U0001F561': {  # 🕡
         'en': ':six-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock630:'],
+        'alias': [':clock630:', ':six_thirty:'],
         'variant': True,
         'de': ':6.30_uhr:',
         'es': ':seis_y_media:',
         'fr': ':six_heures_et_demie:',
         'ja': ':6時半:',
         'ko': ':여섯_시_반:',
         'pt': ':seis_e_meia:',
@@ -51819,15 +52720,15 @@
         'id': ':jam_setengah_tujuh:',
         'zh': ':六点半:'
     },
     '\U0001F555': {  # 🕕
         'en': ':six_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock6:'],
+        'alias': [':clock6:', ':six_oclock:'],
         'variant': True,
         'de': ':6.00_uhr:',
         'es': ':6_en_punto:',
         'fr': ':six_heures:',
         'ja': ':6時:',
         'ko': ':여섯_시:',
         'pt': ':6_horas:',
@@ -52130,15 +53031,15 @@
         'id': ':wajik_oranye_kecil:',
         'zh': ':橙色小菱形:'
     },
     '\U0001F63B': {  # 😻
         'en': ':smiling_cat_with_heart-eyes:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':heart_eyes_cat:'],
+        'alias': [':heart_eyes_cat:', ':smiling_cat_with_heart_eyes:'],
         'de': ':lachende_katze_mit_herzen_als_augen:',
         'es': ':gato_sonriendo_con_ojos_de_corazón:',
         'fr': ':chat_souriant_aux_yeux_en_cœurs:',
         'ja': ':目がハートの猫:',
         'ko': ':하트_눈_고양이_얼굴:',
         'pt': ':rosto_de_gato_sorridente_com_olhos_de_coração:',
         'it': ':gatto_innamorato:',
@@ -52196,15 +53097,15 @@
         'id': ':wajah_malaikat:',
         'zh': ':微笑天使:'
     },
     '\U0001F60D': {  # 😍
         'en': ':smiling_face_with_heart-eyes:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':heart_eyes:'],
+        'alias': [':heart_eyes:', ':smiling_face_with_heart_eyes:'],
         'de': ':lächelndes_gesicht_mit_herzförmigen_augen:',
         'es': ':cara_sonriendo_con_ojos_de_corazón:',
         'fr': ':visage_souriant_avec_yeux_en_forme_de_cœur:',
         'ja': ':目がハートの笑顔:',
         'ko': ':하트_눈_얼굴:',
         'pt': ':rosto_sorridente_com_olhos_de_coração:',
         'it': ':faccina_con_sorriso_e_occhi_a_cuore:',
@@ -52780,15 +53681,15 @@
         'id': ':hati_bersinar:',
         'zh': ':闪亮的心:'
     },
     '\U0001F64A': {  # 🙊
         'en': ':speak-no-evil_monkey:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':speak_no_evil:'],
+        'alias': [':speak_no_evil:', ':speak_no_evil_monkey:'],
         'de': ':sich_den_mund_zuhaltendes_affengesicht:',
         'es': ':mono_con_la_boca_tapada:',
         'fr': ':singe_ne_rien_dire:',
         'ja': ':言わざる:',
         'ko': ':입을_막고_있는_원숭이:',
         'pt': ':macaco_que_não_fala_nada:',
         'it': ':non_parlo:',
@@ -54124,15 +55025,15 @@
         'id': ':suntikan:',
         'zh': ':注射器:'
     },
     '\U0001F455': {  # 👕
         'en': ':t-shirt:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':tshirt:', ':shirt:'],
+        'alias': [':tshirt:', ':shirt:', ':t_shirt:'],
         'de': ':t-shirt:',
         'es': ':camiseta:',
         'fr': ':t-shirt:',
         'ja': ':tシャツ:',
         'ko': ':티셔츠:',
         'pt': ':camiseta:',
         'it': ':t-shirt:',
@@ -54352,15 +55253,15 @@
         'id': ':teko:',
         'zh': ':茶壶:'
     },
     '\U0001F4C6': {  # 📆
         'en': ':tear-off_calendar:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':calendar:'],
+        'alias': [':calendar:', ':tear_off_calendar:'],
         'de': ':abreißkalender:',
         'es': ':calendario_recortable:',
         'fr': ':éphéméride:',
         'ja': ':日めくりカレンダー:',
         'ko': ':뜯어진_달력:',
         'pt': ':calendário_com_folhas_destacáveis:',
         'it': ':calendario_a_strappo:',
@@ -54554,15 +55455,15 @@
         'id': ':televisi:',
         'zh': ':电视机:'
     },
     '\U0001F565': {  # 🕥
         'en': ':ten-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock1030:'],
+        'alias': [':clock1030:', ':ten_thirty:'],
         'variant': True,
         'de': ':10.30_uhr:',
         'es': ':diez_y_media:',
         'fr': ':dix_heures_et_demie:',
         'ja': ':10時半:',
         'ko': ':열_시_반:',
         'pt': ':dez_e_meia:',
@@ -54571,15 +55472,15 @@
         'id': ':jam_setengah_sebelas:',
         'zh': ':十点半:'
     },
     '\U0001F559': {  # 🕙
         'en': ':ten_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock10:'],
+        'alias': [':clock10:', ':ten_oclock:'],
         'variant': True,
         'de': ':10.00_uhr:',
         'es': ':10_en_punto:',
         'fr': ':dix_heures:',
         'ja': ':10時:',
         'ko': ':열_시:',
         'pt': ':10_horas:',
@@ -54727,15 +55628,15 @@
         'id': ':benang:',
         'zh': ':线:'
     },
     '\U0001F55E': {  # 🕞
         'en': ':three-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock330:'],
+        'alias': [':clock330:', ':three_thirty:'],
         'variant': True,
         'de': ':3.30_uhr:',
         'es': ':tres_y_media:',
         'fr': ':trois_heures_et_demie:',
         'ja': ':3時半:',
         'ko': ':세_시_반:',
         'pt': ':três_e_meia:',
@@ -54744,15 +55645,15 @@
         'id': ':jam_setengah_empat:',
         'zh': ':三点半:'
     },
     '\U0001F552': {  # 🕒
         'en': ':three_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock3:'],
+        'alias': [':clock3:', ':three_oclock:'],
         'variant': True,
         'de': ':3.00_uhr:',
         'es': ':3_en_punto:',
         'fr': ':trois_heures:',
         'ja': ':3時:',
         'ko': ':세_시:',
         'pt': ':3_horas:',
@@ -55597,15 +56498,15 @@
         'id': ':kura-kura:',
         'zh': ':龟:'
     },
     '\U0001F567': {  # 🕧
         'en': ':twelve-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock1230:'],
+        'alias': [':clock1230:', ':twelve_thirty:'],
         'variant': True,
         'de': ':12.30_uhr:',
         'es': ':doce_y_media:',
         'fr': ':midi/minuit_et_demie:',
         'ja': ':12時半:',
         'ko': ':열두_시_반:',
         'pt': ':doze_e_meia:',
@@ -55614,15 +56515,15 @@
         'id': ':jam_setengah_satu:',
         'zh': ':十二点半:'
     },
     '\U0001F55B': {  # 🕛
         'en': ':twelve_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock12:'],
+        'alias': [':clock12:', ':twelve_oclock:'],
         'variant': True,
         'de': ':ziffernblatt_12.00_uhr:',
         'es': ':12_en_punto:',
         'fr': ':midi/minuit:',
         'ja': ':12時:',
         'ko': ':열두_시:',
         'pt': ':12_horas:',
@@ -55631,15 +56532,15 @@
         'id': ':jam_dua_belas_tepat:',
         'zh': ':十二点:'
     },
     '\U0001F42B': {  # 🐫
         'en': ':two-hump_camel:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':camel:'],
+        'alias': [':camel:', ':two_hump_camel:'],
         'de': ':kamel:',
         'es': ':camello:',
         'fr': ':chameau:',
         'ja': ':フタコブラクダ:',
         'ko': ':쌍봉_낙타:',
         'pt': ':camelo_com_duas_corcovas:',
         'it': ':cammello:',
@@ -55647,15 +56548,15 @@
         'id': ':unta_berpunuk_dua:',
         'zh': ':双峰骆驼:'
     },
     '\U0001F55D': {  # 🕝
         'en': ':two-thirty:',
         'status': fully_qualified,
         'E': 0.7,
-        'alias': [':clock230:'],
+        'alias': [':clock230:', ':two_thirty:'],
         'variant': True,
         'de': ':2.30_uhr:',
         'es': ':dos_y_media:',
         'fr': ':deux_heures_et_demie:',
         'ja': ':2時半:',
         'ko': ':두_시_반:',
         'pt': ':duas_e_meia:',
@@ -55679,15 +56580,15 @@
         'id': ':dua_hati:',
         'zh': ':两颗心:'
     },
     '\U0001F551': {  # 🕑
         'en': ':two_o’clock:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':clock2:'],
+        'alias': [':clock2:', ':two_oclock:'],
         'variant': True,
         'de': ':2.00_uhr:',
         'es': ':2_en_punto:',
         'fr': ':deux_heures:',
         'ja': ':2時:',
         'ko': ':두_시:',
         'pt': ':2_horas:',
@@ -55830,15 +56731,15 @@
         'id': ':gembok_terbuka:',
         'zh': ':打开的锁:'
     },
     '\U00002195\U0000FE0F': {  # ↕️
         'en': ':up-down_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':arrow_up_down:'],
+        'alias': [':arrow_up_down:', ':up_down_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_oben_und_unten:',
         'es': ':flecha_arriba_y_abajo:',
         'fr': ':flèche_haut_bas:',
         'ja': ':上下矢印:',
         'ko': ':상하향_화살표:',
         'pt': ':seta_para_cima_e_para_baixo:',
@@ -55847,15 +56748,15 @@
         'id': ':tanda_panah_atas_bawah:',
         'zh': ':上下箭头:'
     },
     '\U00002195': {  # ↕
         'en': ':up-down_arrow:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':arrow_up_down:'],
+        'alias': [':arrow_up_down:', ':up_down_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_oben_und_unten:',
         'es': ':flecha_arriba_y_abajo:',
         'fr': ':flèche_haut_bas:',
         'ja': ':上下矢印:',
         'ko': ':상하향_화살표:',
         'pt': ':seta_para_cima_e_para_baixo:',
@@ -55864,15 +56765,15 @@
         'id': ':tanda_panah_atas_bawah:',
         'zh': ':上下箭头:'
     },
     '\U00002196\U0000FE0F': {  # ↖️
         'en': ':up-left_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':arrow_upper_left:'],
+        'alias': [':arrow_upper_left:', ':up_left_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_links_oben:',
         'es': ':flecha_hacia_la_esquina_superior_izquierda:',
         'fr': ':flèche_haut_gauche:',
         'ja': ':左上矢印:',
         'ko': ':좌상향_화살표:',
         'pt': ':seta_para_cima_e_para_a_esquerda:',
@@ -55881,15 +56782,15 @@
         'id': ':tanda_panah_kiri_atas:',
         'zh': ':左上箭头:'
     },
     '\U00002196': {  # ↖
         'en': ':up-left_arrow:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':arrow_upper_left:'],
+        'alias': [':arrow_upper_left:', ':up_left_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_links_oben:',
         'es': ':flecha_hacia_la_esquina_superior_izquierda:',
         'fr': ':flèche_haut_gauche:',
         'ja': ':左上矢印:',
         'ko': ':좌상향_화살표:',
         'pt': ':seta_para_cima_e_para_a_esquerda:',
@@ -55898,15 +56799,15 @@
         'id': ':tanda_panah_kiri_atas:',
         'zh': ':左上箭头:'
     },
     '\U00002197\U0000FE0F': {  # ↗️
         'en': ':up-right_arrow:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':arrow_upper_right:'],
+        'alias': [':arrow_upper_right:', ':up_right_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_rechts_oben:',
         'es': ':flecha_hacia_la_esquina_superior_derecha:',
         'fr': ':flèche_haut_droite:',
         'ja': ':右上矢印:',
         'ko': ':우상향_화살표:',
         'pt': ':seta_para_cima_e_para_a_direita:',
@@ -55915,15 +56816,15 @@
         'id': ':tanda_panah_kanan_atas:',
         'zh': ':右上箭头:'
     },
     '\U00002197': {  # ↗
         'en': ':up-right_arrow:',
         'status': unqualified,
         'E': 0.6,
-        'alias': [':arrow_upper_right:'],
+        'alias': [':arrow_upper_right:', ':up_right_arrow:'],
         'variant': True,
         'de': ':pfeil_nach_rechts_oben:',
         'es': ':flecha_hacia_la_esquina_superior_derecha:',
         'fr': ':flèche_haut_droite:',
         'ja': ':右上矢印:',
         'ko': ':우상향_화살표:',
         'pt': ':seta_para_cima_e_para_a_direita:',
@@ -60771,15 +61672,15 @@
         'id': ':jin_wanita:',
         'zh': ':女妖怪:'
     },
     '\U0001F645\U0000200D\U00002640\U0000FE0F': {  # 🙅‍♀️
         'en': ':woman_gesturing_NO:',
         'status': fully_qualified,
         'E': 4,
-        'alias': [':ng_woman:', ':no_good_woman:'],
+        'alias': [':ng_woman:', ':no_good_woman:', ':woman_gesturing_no:'],
         'de': ':frau_mit_überkreuzten_armen:',
         'es': ':mujer_haciendo_el_gesto_de_no:',
         'fr': ':femme_faisant_un_geste_d’interdiction:',
         'ja': ':ダメのポーズをする女:',
         'ko': ':안_된다는_제스처를_하는_여자:',
         'pt': ':mulher_fazendo_gesto_de_“não”:',
         'it': ':donna_con_gesto_di_rifiuto:',
@@ -60787,15 +61688,15 @@
         'id': ':wanita_mengisyaratkan_tidak:',
         'zh': ':禁止手势女:'
     },
     '\U0001F645\U0000200D\U00002640': {  # 🙅‍♀
         'en': ':woman_gesturing_NO:',
         'status': minimally_qualified,
         'E': 4,
-        'alias': [':ng_woman:', ':no_good_woman:'],
+        'alias': [':ng_woman:', ':no_good_woman:', ':woman_gesturing_no:'],
         'de': ':frau_mit_überkreuzten_armen:',
         'es': ':mujer_haciendo_el_gesto_de_no:',
         'fr': ':femme_faisant_un_geste_d’interdiction:',
         'ja': ':ダメのポーズをする女:',
         'ko': ':안_된다는_제스처를_하는_여자:',
         'pt': ':mulher_fazendo_gesto_de_“não”:',
         'it': ':donna_con_gesto_di_rifiuto:',
@@ -60953,15 +61854,15 @@
         'id': ':wanita_mengisyaratkan_tidak_warna_kulit_sedang:',
         'zh': ':禁止手势女_中等肤色:'
     },
     '\U0001F646\U0000200D\U00002640\U0000FE0F': {  # 🙆‍♀️
         'en': ':woman_gesturing_OK:',
         'status': fully_qualified,
         'E': 4,
-        'alias': [':ok_woman:'],
+        'alias': [':ok_woman:', ':woman_gesturing_ok:'],
         'de': ':frau_mit_händen_auf_dem_kopf:',
         'es': ':mujer_haciendo_el_gesto_de_de_acuerdo:',
         'fr': ':femme_faisant_un_geste_d’acceptation:',
         'ja': ':okのポーズをする女:',
         'ko': ':오케이라는_제스처를_하는_여자:',
         'pt': ':mulher_fazendo_gesto_de_“ok”:',
         'it': ':donna_con_gesto_ok:',
@@ -60969,15 +61870,15 @@
         'id': ':wanita_mengisyaratkan_oke:',
         'zh': ':OK手势女:'
     },
     '\U0001F646\U0000200D\U00002640': {  # 🙆‍♀
         'en': ':woman_gesturing_OK:',
         'status': minimally_qualified,
         'E': 4,
-        'alias': [':ok_woman:'],
+        'alias': [':ok_woman:', ':woman_gesturing_ok:'],
         'de': ':frau_mit_händen_auf_dem_kopf:',
         'es': ':mujer_haciendo_el_gesto_de_de_acuerdo:',
         'fr': ':femme_faisant_un_geste_d’acceptation:',
         'ja': ':okのポーズをする女:',
         'ko': ':오케이라는_제스처를_하는_여자:',
         'pt': ':mulher_fazendo_gesto_de_“ok”:',
         'it': ':donna_con_gesto_ok:',
@@ -68784,15 +69685,15 @@
         'id': ':zombi_wanita:',
         'zh': ':女僵尸:'
     },
     '\U0001F462': {  # 👢
         'en': ':woman’s_boot:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':boot:'],
+        'alias': [':boot:', ':womans_boot:'],
         'de': ':damenstiefel:',
         'es': ':bota_de_mujer:',
         'fr': ':botte_de_femme:',
         'ja': ':ブーツ:',
         'ko': ':부츠:',
         'pt': ':bota_feminina:',
         'it': ':stivale_da_donna:',
@@ -68832,15 +69733,15 @@
         'id': ':topi_wanita:',
         'zh': ':女帽:'
     },
     '\U0001F461': {  # 👡
         'en': ':woman’s_sandal:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':sandal:'],
+        'alias': [':sandal:', ':womans_sandal:'],
         'de': ':damensandale:',
         'es': ':sandalia_de_mujer:',
         'fr': ':sandale_de_femme:',
         'ja': ':サンダル:',
         'ko': ':샌들:',
         'pt': ':sandália_feminina:',
         'it': ':sandalo_da_donna:',
@@ -69301,15 +70202,15 @@
         'id': ':wanita_bergulat:',
         'zh': ':女生摔跤:'
     },
     '\U0001F6BA': {  # 🚺
         'en': ':women’s_room:',
         'status': fully_qualified,
         'E': 0.6,
-        'alias': [':womens:'],
+        'alias': [':womens:', ':womens_room:'],
         'variant': True,
         'de': ':damen:',
         'es': ':señal_de_aseo_para_mujeres:',
         'fr': ':symbole_toilettes_femmes:',
         'ja': ':女子トイレ:',
         'ko': ':여자_화장실:',
         'pt': ':banheiro_feminino:',
@@ -69549,14 +70450,15 @@
         'id': ':tangan_menulis_warna_kulit_sedang:',
         'zh': ':写字_中等肤色:'
     },
     '\U0001FA7B': {  # 🩻
         'en': ':x-ray:',
         'status': fully_qualified,
         'E': 14,
+        'alias': [':x_ray:'],
         'de': ':röntgenbild:',
         'es': ':radiografía:',
         'fr': ':radiographie:',
         'ja': ':x線:',
         'ko': ':엑스레이:',
         'pt': ':raio_x:',
         'it': ':radiografia:',
```

### Comparing `emoji-2.6.0/emoji.egg-info/PKG-INFO` & `emoji-2.7.0/emoji.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emoji
-Version: 2.6.0
+Version: 2.7.0
 Summary: Emoji for Python
 Home-page: https://github.com/carpedm20/emoji/
 Author: Taehoon Kim, Kevin Wurster
 Author-email: carpedm20@gmail.com
 License: New BSD
 Keywords: emoji
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `emoji-2.6.0/emoji.egg-info/SOURCES.txt` & `emoji-2.7.0/emoji.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CHANGES.md
 LICENSE.txt
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
 emoji/__init__.py
 emoji/__init__.pyi
 emoji/core.py
 emoji/core.pyi
 emoji/py.typed
```

### Comparing `emoji-2.6.0/setup.py` & `emoji-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_analyze.py` & `emoji-2.7.0/tests/test_analyze.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_core.py` & `emoji-2.7.0/tests/test_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -504,20 +504,20 @@
     assert emoji.demojize(invalidchar) == invalidchar, "%r != %r" % (ascii(emoji.demojize(invalidchar)), ascii(invalidchar))
 
 
 def test_combine_with_component():
     text = "Example of a combined emoji%sin a sentence"
 
     combined = emoji.emojize(text % ":woman_dark_skin_tone:")
-    seperated = emoji.emojize(text % ":woman::dark_skin_tone:")
-    assert combined == seperated,  "%r != %r" % (ascii(combined), ascii(seperated))
+    separated = emoji.emojize(text % ":woman::dark_skin_tone:")
+    assert combined == separated,  "%r != %r" % (ascii(combined), ascii(separated))
 
     combined = emoji.emojize(text % ":woman_dark_skin_tone_white_hair:")
-    seperated = emoji.emojize(text % ":woman::dark_skin_tone:\u200d:white_hair:")
-    assert combined == seperated,  "%r != %r" % (ascii(combined), ascii(seperated))
+    separated = emoji.emojize(text % ":woman::dark_skin_tone:\u200d:white_hair:")
+    assert combined == separated,  "%r != %r" % (ascii(combined), ascii(separated))
 
 
 purely_emoji_testdata = [
     ('\U0001f600\ufe0f', True),
     ('\U0001f600', True),
     ('\U0001f600\U0001f600\U0001f600', True),
     ('abc', False),
```

### Comparing `emoji-2.6.0/tests/test_dict.py` & `emoji-2.7.0/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_nfkc.py` & `emoji-2.7.0/tests/test_nfkc.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_unicode_codes.py` & `emoji-2.7.0/tests/test_unicode_codes.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_versions.py` & `emoji-2.7.0/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_zwj_common.py` & `emoji-2.7.0/tests/test_zwj_common.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_zwj_keep.py` & `emoji-2.7.0/tests/test_zwj_keep.py`

 * *Files identical despite different names*

### Comparing `emoji-2.6.0/tests/test_zwj_remove.py` & `emoji-2.7.0/tests/test_zwj_remove.py`

 * *Files identical despite different names*

