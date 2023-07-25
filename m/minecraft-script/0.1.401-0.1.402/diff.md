# Comparing `tmp/minecraft_script-0.1.401.tar.gz` & `tmp/minecraft_script-0.1.402.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minecraft_script-0.1.401.tar", last modified: Tue Jul 25 18:42:33 2023, max compression
+gzip compressed data, was "minecraft_script-0.1.402.tar", last modified: Tue Jul 25 18:58:21 2023, max compression
```

## Comparing `minecraft_script-0.1.401.tar` & `minecraft_script-0.1.402.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-25 18:42:33.972825 minecraft_script-0.1.401/
--rw-rw-rw-   0        0        0     3188 2023-07-25 18:42:33.972825 minecraft_script-0.1.401/PKG-INFO
--rw-rw-rw-   0        0        0     2697 2023-07-25 18:41:58.000000 minecraft_script-0.1.401/README.md
-drwxrwxrwx   0        0        0        0 2023-07-25 18:42:33.957291 minecraft_script-0.1.401/minecraft_script/
--rw-rw-rw-   0        0        0     1401 2023-07-25 18:37:26.000000 minecraft_script-0.1.401/minecraft_script/__init__.py
--rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.401/minecraft_script/__main__.py
--rw-rw-rw-   0        0        0     1749 2023-07-20 20:24:19.000000 minecraft_script-0.1.401/minecraft_script/builder.py
--rw-rw-rw-   0        0        0       51 2023-07-20 19:42:42.000000 minecraft_script-0.1.401/minecraft_script/common.py
--rw-rw-rw-   0        0        0     1809 2023-07-25 15:57:38.000000 minecraft_script-0.1.401/minecraft_script/errors.py
--rw-rw-rw-   0        0        0     4311 2023-07-25 18:26:05.000000 minecraft_script-0.1.401/minecraft_script/interpreter.py
--rw-rw-rw-   0        0        0     3763 2023-07-25 18:29:48.000000 minecraft_script-0.1.401/minecraft_script/lexer.py
--rw-rw-rw-   0        0        0     2922 2023-07-25 18:24:44.000000 minecraft_script-0.1.401/minecraft_script/nodes.py
--rw-rw-rw-   0        0        0     5700 2023-07-25 18:29:48.000000 minecraft_script-0.1.401/minecraft_script/parser.py
--rw-rw-rw-   0        0        0     2084 2023-07-25 18:37:26.000000 minecraft_script-0.1.401/minecraft_script/shell_commands.py
--rw-rw-rw-   0        0        0     1143 2023-07-20 14:14:30.000000 minecraft_script-0.1.401/minecraft_script/text_additions.py
--rw-rw-rw-   0        0        0      211 2023-07-20 15:18:51.000000 minecraft_script-0.1.401/minecraft_script/tokens.py
--rw-rw-rw-   0        0        0     2843 2023-07-25 18:21:13.000000 minecraft_script-0.1.401/minecraft_script/types.py
-drwxrwxrwx   0        0        0        0 2023-07-25 18:42:33.971933 minecraft_script-0.1.401/minecraft_script.egg-info/
--rw-rw-rw-   0        0        0     3188 2023-07-25 18:42:33.000000 minecraft_script-0.1.401/minecraft_script.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      552 2023-07-25 18:42:33.000000 minecraft_script-0.1.401/minecraft_script.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-25 18:42:33.000000 minecraft_script-0.1.401/minecraft_script.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-07-25 18:42:33.000000 minecraft_script-0.1.401/minecraft_script.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-25 18:42:33.973827 minecraft_script-0.1.401/setup.cfg
--rw-rw-rw-   0        0        0      880 2023-07-20 15:44:39.000000 minecraft_script-0.1.401/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:58:21.831487 minecraft_script-0.1.402/
+-rw-rw-rw-   0        0        0     3188 2023-07-25 18:58:21.830485 minecraft_script-0.1.402/PKG-INFO
+-rw-rw-rw-   0        0        0     2697 2023-07-25 18:41:58.000000 minecraft_script-0.1.402/README.md
+drwxrwxrwx   0        0        0        0 2023-07-25 18:58:21.811729 minecraft_script-0.1.402/minecraft_script/
+-rw-rw-rw-   0        0        0     1401 2023-07-25 18:57:58.000000 minecraft_script-0.1.402/minecraft_script/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-07-19 19:22:33.000000 minecraft_script-0.1.402/minecraft_script/__main__.py
+-rw-rw-rw-   0        0        0     2276 2023-07-25 18:56:13.000000 minecraft_script-0.1.402/minecraft_script/builder.py
+-rw-rw-rw-   0        0        0       51 2023-07-20 19:42:42.000000 minecraft_script-0.1.402/minecraft_script/common.py
+-rw-rw-rw-   0        0        0     1809 2023-07-25 15:57:38.000000 minecraft_script-0.1.402/minecraft_script/errors.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:58:21.830485 minecraft_script-0.1.402/minecraft_script/grammar/
+-rw-rw-rw-   0        0        0       88 2023-07-25 16:40:21.000000 minecraft_script-0.1.402/minecraft_script/grammar/LANG_KEYWORDS.json
+-rw-rw-rw-   0        0        0      382 2023-07-25 17:17:44.000000 minecraft_script-0.1.402/minecraft_script/grammar/LANG_TOKENS.json
+-rw-rw-rw-   0        0        0     4311 2023-07-25 18:26:05.000000 minecraft_script-0.1.402/minecraft_script/interpreter.py
+-rw-rw-rw-   0        0        0     3763 2023-07-25 18:29:48.000000 minecraft_script-0.1.402/minecraft_script/lexer.py
+-rw-rw-rw-   0        0        0     2922 2023-07-25 18:24:44.000000 minecraft_script-0.1.402/minecraft_script/nodes.py
+-rw-rw-rw-   0        0        0     5700 2023-07-25 18:29:48.000000 minecraft_script-0.1.402/minecraft_script/parser.py
+-rw-rw-rw-   0        0        0     2084 2023-07-25 18:37:26.000000 minecraft_script-0.1.402/minecraft_script/shell_commands.py
+-rw-rw-rw-   0        0        0     1143 2023-07-20 14:14:30.000000 minecraft_script-0.1.402/minecraft_script/text_additions.py
+-rw-rw-rw-   0        0        0      211 2023-07-20 15:18:51.000000 minecraft_script-0.1.402/minecraft_script/tokens.py
+-rw-rw-rw-   0        0        0     2843 2023-07-25 18:21:13.000000 minecraft_script-0.1.402/minecraft_script/types.py
+drwxrwxrwx   0        0        0        0 2023-07-25 18:58:21.828483 minecraft_script-0.1.402/minecraft_script.egg-info/
+-rw-rw-rw-   0        0        0     3188 2023-07-25 18:58:21.000000 minecraft_script-0.1.402/minecraft_script.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      638 2023-07-25 18:58:21.000000 minecraft_script-0.1.402/minecraft_script.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-25 18:58:21.000000 minecraft_script-0.1.402/minecraft_script.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-07-25 18:58:21.000000 minecraft_script-0.1.402/minecraft_script.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-25 18:58:21.831487 minecraft_script-0.1.402/setup.cfg
+-rw-rw-rw-   0        0        0      980 2023-07-25 18:58:05.000000 minecraft_script-0.1.402/setup.py
```

### Comparing `minecraft_script-0.1.401/PKG-INFO` & `minecraft_script-0.1.402/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft_script
-Version: 0.1.401
+Version: 0.1.402
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.401/README.md` & `minecraft_script-0.1.402/README.md`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/__init__.py` & `minecraft_script-0.1.402/minecraft_script/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .lexer import Lexer
 from .parser import Parser
 from .interpreter import Interpreter, Context, SymbolTable
 
-version = "0.1.401"
+version = "0.1.402"
 
 
 def run(text: str):
     global_symbol_table = SymbolTable()
 
     run_lexer = Lexer(text)
     tokens = run_lexer.tokenize()
```

### Comparing `minecraft_script-0.1.401/minecraft_script/errors.py` & `minecraft_script-0.1.402/minecraft_script/errors.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/interpreter.py` & `minecraft_script-0.1.402/minecraft_script/interpreter.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/lexer.py` & `minecraft_script-0.1.402/minecraft_script/lexer.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/nodes.py` & `minecraft_script-0.1.402/minecraft_script/nodes.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/parser.py` & `minecraft_script-0.1.402/minecraft_script/parser.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/shell_commands.py` & `minecraft_script-0.1.402/minecraft_script/shell_commands.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/text_additions.py` & `minecraft_script-0.1.402/minecraft_script/text_additions.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script/types.py` & `minecraft_script-0.1.402/minecraft_script/types.py`

 * *Files identical despite different names*

### Comparing `minecraft_script-0.1.401/minecraft_script.egg-info/PKG-INFO` & `minecraft_script-0.1.402/minecraft_script.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minecraft-script
-Version: 0.1.401
+Version: 0.1.402
 Summary: Minecraft Script Programming language
 Author: Joyful-Bard
 Author-email: <thisis@notarealemail.com>
 Keywords: minecraft,mc,script,language
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Microsoft :: Windows
```

### Comparing `minecraft_script-0.1.401/minecraft_script.egg-info/SOURCES.txt` & `minecraft_script-0.1.402/minecraft_script.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -12,8 +12,10 @@
 minecraft_script/shell_commands.py
 minecraft_script/text_additions.py
 minecraft_script/tokens.py
 minecraft_script/types.py
 minecraft_script.egg-info/PKG-INFO
 minecraft_script.egg-info/SOURCES.txt
 minecraft_script.egg-info/dependency_links.txt
-minecraft_script.egg-info/top_level.txt
+minecraft_script.egg-info/top_level.txt
+minecraft_script/grammar/LANG_KEYWORDS.json
+minecraft_script/grammar/LANG_TOKENS.json
```

### Comparing `minecraft_script-0.1.401/setup.py` & `minecraft_script-0.1.402/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.401'
+VERSION = '0.1.402'
 DESCRIPTION = 'Minecraft Script Programming language'
 
 # Setting up
 setup(
     name="minecraft_script",
     version=VERSION,
     author="Joyful-Bard",
     author_email="<thisis@notarealemail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
+    package_data={'minecraft_script': ['grammar/LANG_TOKENS.json', 'grammar/LANG_KEYWORDS.json']},
     install_requires=[],
     keywords=['minecraft', 'mc', 'script', 'language'],
     classifiers=[
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
```

