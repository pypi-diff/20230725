# Comparing `tmp/easy-email-builder-1.0.1.tar.gz` & `tmp/easy-email-builder-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-email-builder-1.0.1.tar", last modified: Tue Jul 25 19:28:07 2023, max compression
+gzip compressed data, was "easy-email-builder-1.0.2.tar", last modified: Tue Jul 25 19:43:41 2023, max compression
```

## Comparing `easy-email-builder-1.0.1.tar` & `easy-email-builder-1.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/easy_email_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/email_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/email_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/email_builder/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/easy_email_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/email_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/email_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/email_builder/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/setup.py
```

### Comparing `easy-email-builder-1.0.1/PKG-INFO` & `easy-email-builder-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-email-builder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple interface for sending emails with the builder design pattern with different services.
 Author: Ryan Schreiber
 Author-email: ryanschreiber86@gmail.com
 Project-URL: Documentation, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Source, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Tracker, https://github.com/ryan-schreiber/email-builder/issues
 Keywords: email emails builder smtp gmail ses aws
@@ -32,15 +32,16 @@
 ```
 
 #### Send an email from Gmail
 
 ```python
 # builder syntax
 # when using gmail, you need an "App Password". follow this link if you need help creating that:
-# 
+# https://www.lifewire.com/get-a-password-to-access-gmail-by-pop-imap-2-1171882
+
 import email_builder
 
 client = email_builder.clients.Gmail(password="<gmail APP password>")
 email = (
   email_builder.Email()
     .sender("your.email@gmail.com")
     .to("someones.email@gmail.com")
@@ -52,15 +53,15 @@
 email.send(client)
 ```
 
 #### Send an email Amazon SES with just some html as the body
 
 ```python
 # builder syntax 
-import etl_utils
+import email_builder
 
 # this SES class accepts a boto3 session if you want to customize the setup
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
@@ -74,15 +75,15 @@
 #### Send an email with attachments
 
 ```python
 # note that the contents of the attachments can be either string or bytestring 
 import email_builder
 
 with open("report.csv", "rb") as f:
-  report_data = f.read()
+  data = f.read()
 
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
@@ -94,26 +95,29 @@
 ```
 
 ## Email Options
 
 ```python
 import email_builder
 
-# --- client types are SES or Gmail --- #
+with open("report.csv", "rb") as f:
+  data = f.read()
 
+# --- client types are SES or Gmail --- #
 # Amazon SES that can accept a session object as needed
 client = email_builder.clients.SES()
-#or
+# or
 import boto3
-session = boto3.Session(...)
+session = boto3.Session(region="us-west-2", etc)
 client = email_builder.clients.SES(session)
 
 # Gmail that accepts a password and options to configure port/url if needed
 client = email_builder.clients.SES(password="<password>")
 
+
 # --- email options --- #
 email = (
   email_builder.Email()
 
     # sender(sender:str) -> only one sender allowed, no chaining allowed on sender
     .sender("my.email@company.com")
 
@@ -132,15 +136,15 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # need to choose between either html or text, can't use both
+    # you need to choose between either html or text, can't use both
 
     # html(body:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
@@ -150,7 +154,23 @@
 
 )
 
 # result contains a dictionary with status in the body
 result = email.send(client)
 print(result)
 ```
+
+Success result:
+```python
+{
+	"status": "passed",
+	"error": None
+}
+```
+
+Failure result:
+```python
+{
+	"status": "failed",
+	"error": Exception(...)
+}
+```
```

### Comparing `easy-email-builder-1.0.1/README.md` & `easy-email-builder-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 ```
 
 #### Send an email from Gmail
 
 ```python
 # builder syntax
 # when using gmail, you need an "App Password". follow this link if you need help creating that:
-# 
+# https://www.lifewire.com/get-a-password-to-access-gmail-by-pop-imap-2-1171882
+
 import email_builder
 
 client = email_builder.clients.Gmail(password="<gmail APP password>")
 email = (
   email_builder.Email()
     .sender("your.email@gmail.com")
     .to("someones.email@gmail.com")
@@ -37,15 +38,15 @@
 email.send(client)
 ```
 
 #### Send an email Amazon SES with just some html as the body
 
 ```python
 # builder syntax 
-import etl_utils
+import email_builder
 
 # this SES class accepts a boto3 session if you want to customize the setup
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
@@ -59,15 +60,15 @@
 #### Send an email with attachments
 
 ```python
 # note that the contents of the attachments can be either string or bytestring 
 import email_builder
 
 with open("report.csv", "rb") as f:
-  report_data = f.read()
+  data = f.read()
 
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
@@ -79,26 +80,29 @@
 ```
 
 ## Email Options
 
 ```python
 import email_builder
 
-# --- client types are SES or Gmail --- #
+with open("report.csv", "rb") as f:
+  data = f.read()
 
+# --- client types are SES or Gmail --- #
 # Amazon SES that can accept a session object as needed
 client = email_builder.clients.SES()
-#or
+# or
 import boto3
-session = boto3.Session(...)
+session = boto3.Session(region="us-west-2", etc)
 client = email_builder.clients.SES(session)
 
 # Gmail that accepts a password and options to configure port/url if needed
 client = email_builder.clients.SES(password="<password>")
 
+
 # --- email options --- #
 email = (
   email_builder.Email()
 
     # sender(sender:str) -> only one sender allowed, no chaining allowed on sender
     .sender("my.email@company.com")
 
@@ -117,15 +121,15 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # need to choose between either html or text, can't use both
+    # you need to choose between either html or text, can't use both
 
     # html(body:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
@@ -135,7 +139,23 @@
 
 )
 
 # result contains a dictionary with status in the body
 result = email.send(client)
 print(result)
 ```
+
+Success result:
+```python
+{
+	"status": "passed",
+	"error": None
+}
+```
+
+Failure result:
+```python
+{
+	"status": "failed",
+	"error": Exception(...)
+}
+```
```

### Comparing `easy-email-builder-1.0.1/easy_email_builder.egg-info/PKG-INFO` & `easy-email-builder-1.0.2/easy_email_builder.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-email-builder
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple interface for sending emails with the builder design pattern with different services.
 Author: Ryan Schreiber
 Author-email: ryanschreiber86@gmail.com
 Project-URL: Documentation, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Source, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Tracker, https://github.com/ryan-schreiber/email-builder/issues
 Keywords: email emails builder smtp gmail ses aws
@@ -32,15 +32,16 @@
 ```
 
 #### Send an email from Gmail
 
 ```python
 # builder syntax
 # when using gmail, you need an "App Password". follow this link if you need help creating that:
-# 
+# https://www.lifewire.com/get-a-password-to-access-gmail-by-pop-imap-2-1171882
+
 import email_builder
 
 client = email_builder.clients.Gmail(password="<gmail APP password>")
 email = (
   email_builder.Email()
     .sender("your.email@gmail.com")
     .to("someones.email@gmail.com")
@@ -52,15 +53,15 @@
 email.send(client)
 ```
 
 #### Send an email Amazon SES with just some html as the body
 
 ```python
 # builder syntax 
-import etl_utils
+import email_builder
 
 # this SES class accepts a boto3 session if you want to customize the setup
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
@@ -74,15 +75,15 @@
 #### Send an email with attachments
 
 ```python
 # note that the contents of the attachments can be either string or bytestring 
 import email_builder
 
 with open("report.csv", "rb") as f:
-  report_data = f.read()
+  data = f.read()
 
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
@@ -94,26 +95,29 @@
 ```
 
 ## Email Options
 
 ```python
 import email_builder
 
-# --- client types are SES or Gmail --- #
+with open("report.csv", "rb") as f:
+  data = f.read()
 
+# --- client types are SES or Gmail --- #
 # Amazon SES that can accept a session object as needed
 client = email_builder.clients.SES()
-#or
+# or
 import boto3
-session = boto3.Session(...)
+session = boto3.Session(region="us-west-2", etc)
 client = email_builder.clients.SES(session)
 
 # Gmail that accepts a password and options to configure port/url if needed
 client = email_builder.clients.SES(password="<password>")
 
+
 # --- email options --- #
 email = (
   email_builder.Email()
 
     # sender(sender:str) -> only one sender allowed, no chaining allowed on sender
     .sender("my.email@company.com")
 
@@ -132,15 +136,15 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # need to choose between either html or text, can't use both
+    # you need to choose between either html or text, can't use both
 
     # html(body:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
@@ -150,7 +154,23 @@
 
 )
 
 # result contains a dictionary with status in the body
 result = email.send(client)
 print(result)
 ```
+
+Success result:
+```python
+{
+	"status": "passed",
+	"error": None
+}
+```
+
+Failure result:
+```python
+{
+	"status": "failed",
+	"error": Exception(...)
+}
+```
```

### Comparing `easy-email-builder-1.0.1/email_builder/__init__.py` & `easy-email-builder-1.0.2/email_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-email-builder-1.0.1/email_builder/clients.py` & `easy-email-builder-1.0.2/email_builder/clients.py`

 * *Files identical despite different names*

### Comparing `easy-email-builder-1.0.1/setup.py` & `easy-email-builder-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().split("\n")
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='easy-email-builder',
-    version='1.0.1',
+    version='1.0.2',
     description='Simple interface for sending emails with the builder design pattern with different services.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ryan Schreiber',
     author_email='ryanschreiber86@gmail.com',
     packages=find_packages(),
     install_requires=requirements,
```

