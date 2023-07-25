# Comparing `tmp/iamlistening-3.0.1.tar.gz` & `tmp/iamlistening-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iamlistening-3.0.1.tar", max compression
+gzip compressed data, was "iamlistening-3.0.2.tar", max compression
```

## Comparing `iamlistening-3.0.1.tar` & `iamlistening-3.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1064 2023-07-24 20:15:37.920806 iamlistening-3.0.1/LICENSE
--rw-r--r--   0        0        0     2746 2023-07-24 20:15:37.920806 iamlistening-3.0.1/README.md
--rw-r--r--   0        0        0      122 2023-07-24 20:15:39.348824 iamlistening-3.0.1/iamlistening/__init__.py
--rw-r--r--   0        0        0      661 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/config.py
--rw-r--r--   0        0        0     2722 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/default_settings.toml
--rw-r--r--   0        0        0     1660 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/main.py
--rw-r--r--   0        0        0        0 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/platform/__init__.py
--rw-r--r--   0        0        0      761 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/platform/discord.py
--rw-r--r--   0        0        0     1489 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/platform/matrix.py
--rw-r--r--   0        0        0      609 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/platform/rocket_chat.py
--rw-r--r--   0        0        0      808 2023-07-24 20:15:37.920806 iamlistening-3.0.1/iamlistening/platform/telegram.py
--rw-r--r--   0        0        0     3198 2023-07-24 20:15:39.340824 iamlistening-3.0.1/pyproject.toml
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 iamlistening-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-25 15:31:53.820480 iamlistening-3.0.2/LICENSE
+-rw-r--r--   0        0        0     2746 2023-07-25 15:31:53.820480 iamlistening-3.0.2/README.md
+-rw-r--r--   0        0        0      136 2023-07-25 15:31:56.152507 iamlistening-3.0.2/iamlistening/__init__.py
+-rw-r--r--   0        0        0      661 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/config.py
+-rw-r--r--   0        0        0     2722 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/default_settings.toml
+-rw-r--r--   0        0        0     1660 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/main.py
+-rw-r--r--   0        0        0      151 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/__init__.py
+-rw-r--r--   0        0        0      761 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/discord.py
+-rw-r--r--   0        0        0     1489 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/matrix.py
+-rw-r--r--   0        0        0      609 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/rocket_chat.py
+-rw-r--r--   0        0        0      808 2023-07-25 15:31:53.820480 iamlistening-3.0.2/iamlistening/platform/telegram.py
+-rw-r--r--   0        0        0     3198 2023-07-25 15:31:56.144507 iamlistening-3.0.2/pyproject.toml
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 iamlistening-3.0.2/PKG-INFO
```

### Comparing `iamlistening-3.0.1/LICENSE` & `iamlistening-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/README.md` & `iamlistening-3.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/config.py` & `iamlistening-3.0.2/iamlistening/config.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/default_settings.toml` & `iamlistening-3.0.2/iamlistening/default_settings.toml`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/main.py` & `iamlistening-3.0.2/iamlistening/main.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/platform/discord.py` & `iamlistening-3.0.2/iamlistening/platform/discord.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/platform/matrix.py` & `iamlistening-3.0.2/iamlistening/platform/matrix.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/platform/rocket_chat.py` & `iamlistening-3.0.2/iamlistening/platform/rocket_chat.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/iamlistening/platform/telegram.py` & `iamlistening-3.0.2/iamlistening/platform/telegram.py`

 * *Files identical despite different names*

### Comparing `iamlistening-3.0.1/pyproject.toml` & `iamlistening-3.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "iamlistening"
-version = "3.0.1"
+version = "3.0.2"
 description = "A python package to interact with messaging platform."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = [
     "bot","messaging",
     "discord", "telegram","matrix","rocket chat",
```

### Comparing `iamlistening-3.0.1/PKG-INFO` & `iamlistening-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iamlistening
-Version: 3.0.1
+Version: 3.0.2
 Summary: A python package to interact with messaging platform.
 License: MIT
 Keywords: bot,messaging,discord,telegram,matrix,rocket chat
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: iamlistening Version: 3.0.1 Summary: A python
+Metadata-Version: 2.1 Name: iamlistening Version: 3.0.2 Summary: A python
 package to interact with messaging platform. License: MIT Keywords:
 bot,messaging,discord,telegram,matrix,rocket chat Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: loguru (>=0.7.0,<0.8.0) Requires-Dist: py-cord
```

