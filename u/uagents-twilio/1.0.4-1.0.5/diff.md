# Comparing `tmp/uagents_twilio-1.0.4.tar.gz` & `tmp/uagents_twilio-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio-1.0.4.tar", max compression
+gzip compressed data, was "uagents_twilio-1.0.5.tar", max compression
```

## Comparing `uagents_twilio-1.0.4.tar` & `uagents_twilio-1.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.4/LICENSE
--rw-r--r--   0        0        0      576 2023-07-19 05:23:13.567133 uagents_twilio-1.0.4/README.rst
--rw-r--r--   0        0        0      872 2023-07-24 13:59:09.243494 uagents_twilio-1.0.4/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.4/uagents_twilio/__init__.py
--rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio-1.0.4/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.4/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio-1.0.4/uagents_twilio/protocols/messages.py
--rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.4/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio-1.0.4/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     1584 1970-01-01 00:00:00.000000 uagents_twilio-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/LICENSE
+-rw-r--r--   0        0        0     1390 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/README.rst
+-rw-r--r--   0        0        0      928 2023-07-25 05:24:44.293801 uagents_twilio-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/protocols/messages.py
+-rw-r--r--   0        0        0        0 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 uagents_twilio-1.0.5/PKG-INFO
```

### Comparing `uagents_twilio-1.0.4/LICENSE` & `uagents_twilio-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.4/pyproject.toml` & `uagents_twilio-1.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "uagents-twilio"
 #
-version = '1.0.4'
+version = "1.0.5"
 #
-description = ""
-authors = ["Harsh <harsh@gmail.com>"]
+description = "Use uagents to automate SMS/Whatsapp by twilio"
+authors = ["Harsh <harsh.patel@fetch.ai>"]
 readme = "README.rst"
-repository = "https://github.com/Github User/uagents-twilio"
+repository = "https://github.com/harshpatel199259/uagents_twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
```

### Comparing `uagents_twilio-1.0.4/uagents_twilio/protocols/messages.py` & `uagents_twilio-1.0.5/uagents_twilio/protocols/messages.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.4/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio-1.0.5/uagents_twilio/wrappers/messageWrapper.py`

 * *Files identical despite different names*

