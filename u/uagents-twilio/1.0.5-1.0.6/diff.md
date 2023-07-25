# Comparing `tmp/uagents_twilio-1.0.5.tar.gz` & `tmp/uagents_twilio-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uagents_twilio-1.0.5.tar", max compression
+gzip compressed data, was "uagents_twilio-1.0.6.tar", max compression
```

## Comparing `uagents_twilio-1.0.5.tar` & `uagents_twilio-1.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1073 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/LICENSE
--rw-r--r--   0        0        0     1390 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/README.rst
--rw-r--r--   0        0        0      928 2023-07-25 05:24:44.293801 uagents_twilio-1.0.5/pyproject.toml
--rw-r--r--   0        0        0       69 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/__init__.py
--rw-r--r--   0        0        0      254 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/models.py
--rw-r--r--   0        0        0        0 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/protocols/__init__.py
--rw-r--r--   0        0        0     1692 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/protocols/messages.py
--rw-r--r--   0        0        0        0 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/wrappers/__init__.py
--rw-r--r--   0        0        0     1784 2023-07-25 05:24:20.729968 uagents_twilio-1.0.5/uagents_twilio/wrappers/messageWrapper.py
--rw-r--r--   0        0        0     2459 1970-01-01 00:00:00.000000 uagents_twilio-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 08:13:30.274276 uagents_twilio-1.0.6/LICENSE
+-rw-r--r--   0        0        0     1398 2023-07-25 05:51:15.400793 uagents_twilio-1.0.6/README.rst
+-rw-r--r--   0        0        0      928 2023-07-25 05:52:44.948171 uagents_twilio-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-07-24 10:33:08.046614 uagents_twilio-1.0.6/uagents_twilio/__init__.py
+-rw-r--r--   0        0        0      254 2023-07-24 13:21:08.651334 uagents_twilio-1.0.6/uagents_twilio/models.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.290264 uagents_twilio-1.0.6/uagents_twilio/protocols/__init__.py
+-rw-r--r--   0        0        0     1692 2023-07-24 13:50:14.135064 uagents_twilio-1.0.6/uagents_twilio/protocols/messages.py
+-rw-r--r--   0        0        0        0 2023-07-18 08:13:30.286267 uagents_twilio-1.0.6/uagents_twilio/wrappers/__init__.py
+-rw-r--r--   0        0        0     1784 2023-07-24 13:21:08.655334 uagents_twilio-1.0.6/uagents_twilio/wrappers/messageWrapper.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 uagents_twilio-1.0.6/PKG-INFO
```

### Comparing `uagents_twilio-1.0.5/LICENSE` & `uagents_twilio-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.5/README.rst` & `uagents_twilio-1.0.6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -53,9 +53,9 @@
 
     from uagents_twilio.models import Message, MessageType
 
     @service_agent.on_interval(period=2.0)
     async def send_message(ctx: Context):
         await ctx.send(
             AGENT_ADDRESS,
-            Message(receiver="+918849430206", msg="hello there bob", type=MessageType.sms),
+            Message(receiver="<replace_your_number>", msg="hello there bob", type=MessageType.sms),
         )
```

### Comparing `uagents_twilio-1.0.5/pyproject.toml` & `uagents_twilio-1.0.6/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "uagents-twilio"
 #
-version = "1.0.5"
+version = '1.0.6'
 #
 description = "Use uagents to automate SMS/Whatsapp by twilio"
 authors = ["Harsh <harsh.patel@fetch.ai>"]
 readme = "README.rst"
 repository = "https://github.com/harshpatel199259/uagents_twilio"
 packages = [{include = "uagents_twilio"}]
 classifiers=[
```

### Comparing `uagents_twilio-1.0.5/uagents_twilio/protocols/messages.py` & `uagents_twilio-1.0.6/uagents_twilio/protocols/messages.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.5/uagents_twilio/wrappers/messageWrapper.py` & `uagents_twilio-1.0.6/uagents_twilio/wrappers/messageWrapper.py`

 * *Files identical despite different names*

### Comparing `uagents_twilio-1.0.5/PKG-INFO` & `uagents_twilio-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uagents-twilio
-Version: 1.0.5
+Version: 1.0.6
 Summary: Use uagents to automate SMS/Whatsapp by twilio
 Home-page: https://github.com/harshpatel199259/uagents_twilio
 Author: Harsh
 Author-email: harsh.patel@fetch.ai
 Requires-Python: >=3.8.1,<3.12
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -79,10 +79,10 @@
 
     from uagents_twilio.models import Message, MessageType
 
     @service_agent.on_interval(period=2.0)
     async def send_message(ctx: Context):
         await ctx.send(
             AGENT_ADDRESS,
-            Message(receiver="+918849430206", msg="hello there bob", type=MessageType.sms),
+            Message(receiver="<replace_your_number>", msg="hello there bob", type=MessageType.sms),
         )
```

