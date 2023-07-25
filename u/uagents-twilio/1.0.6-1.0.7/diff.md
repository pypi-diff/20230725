# Comparing `tmp/uagents_twilio-1.0.6.tar.gz` & `tmp/uagents_twilio-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio-1.0.6.tar", max compression
+gzip compressed data, was "uagents_twilio-1.0.7.tar", max compression
```

## Comparing `uagents_twilio-1.0.6.tar` & `uagents_twilio-1.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.6/LICENSE
--rw-r--r--   0        0        0     1398 2023-07-25 05:51:15.400793 uagents_twilio-1.0.6/README.rst
--rw-r--r--   0        0        0      928 2023-07-25 05:52:44.948171 uagents_twilio-1.0.6/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.6/uagents_twilio/__init__.py
--rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio-1.0.6/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.6/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio-1.0.6/uagents_twilio/protocols/messages.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.6/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio-1.0.6/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 uagents_twilio-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.7/LICENSE
+-rw-r--r--   0        0        0     1478 2023-07-25 06:57:41.723405 uagents_twilio-1.0.7/README.rst
+-rw-r--r--   0        0        0      928 2023-07-25 07:01:59.682483 uagents_twilio-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.7/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio-1.0.7/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.7/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio-1.0.7/uagents_twilio/protocols/messages.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.7/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio-1.0.7/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 uagents_twilio-1.0.7/PKG-INFO
```

### Comparing `uagents_twilio-1.0.6/LICENSE` & `uagents_twilio-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.6/README.rst` & `uagents_twilio-1.0.7/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -20,16 +20,19 @@
 
 
 Installation
 ------------
 
 You can install "uagents-twilio" via `pip <https://pypi.org/project/pip/>`_ from `PyPI <https://pypi.org/project>`_::
 
-    $ poetry add uagents-twilio
+    $ pip install uagents-twilio
+
+You can install "uagents_twilio" via poetry::
 
+    $ poetry add uagents-twilio
 
 Usage
 -----
 
 * Create .env file in root folder of project::
 
     AGENT_ADDRESS=""
```

### Comparing `uagents_twilio-1.0.6/pyproject.toml` & `uagents_twilio-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-twilio"
 #
-version = '1.0.6'
+version = '1.0.7'
 #
 description = "Use uagents to automate SMS/Whatsapp by twilio"
 authors = ["Harsh <harsh.patel@fetch.ai>"]
 readme = "README.rst"
 repository = "https://github.com/harshpatel199259/uagents_twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
```

### Comparing `uagents_twilio-1.0.6/uagents_twilio/protocols/messages.py` & `uagents_twilio-1.0.7/uagents_twilio/protocols/messages.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.6/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio-1.0.7/uagents_twilio/wrappers/messageWrapper.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.6/PKG-INFO` & `uagents_twilio-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-twilio
-Version: 1.0.6
+Version: 1.0.7
 Summary: Use uagents to automate SMS/Whatsapp by twilio
 Home-page: https://github.com/harshpatel199259/uagents_twilio
 Author: Harsh
 Author-email: harsh.patel@fetch.ai
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -46,16 +46,19 @@
 
 
 Installation
 ------------
 
 You can install "uagents-twilio" via `pip <https://pypi.org/project/pip/>`_ from `PyPI <https://pypi.org/project>`_::
 
-    $ poetry add uagents-twilio
+    $ pip install uagents-twilio
+
+You can install "uagents_twilio" via poetry::
 
+    $ poetry add uagents-twilio
 
 Usage
 -----
 
 * Create .env file in root folder of project::
 
     AGENT_ADDRESS=""
```

