# Comparing `tmp/easy-email-builder-1.0.2.tar.gz` & `tmp/easy-email-builder-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-email-builder-1.0.2.tar", last modified: Tue Jul 25 19:43:41 2023, max compression
+gzip compressed data, was "easy-email-builder-1.0.3.tar", last modified: Tue Jul 25 19:58:19 2023, max compression
```

## Comparing `easy-email-builder-1.0.2.tar` & `easy-email-builder-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/easy_email_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:43:41.000000 easy-email-builder-1.0.2/easy_email_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/email_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/email_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/email_builder/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:43:41.013562 easy-email-builder-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 19:43:28.000000 easy-email-builder-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:58:19.413206 easy-email-builder-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-25 19:58:19.413206 easy-email-builder-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-07-25 19:58:09.000000 easy-email-builder-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:58:19.413206 easy-email-builder-1.0.3/easy_email_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-25 19:58:19.000000 easy-email-builder-1.0.3/easy_email_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 19:58:19.000000 easy-email-builder-1.0.3/easy_email_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:58:19.000000 easy-email-builder-1.0.3/easy_email_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 19:58:19.000000 easy-email-builder-1.0.3/easy_email_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:58:19.000000 easy-email-builder-1.0.3/easy_email_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:58:19.413206 easy-email-builder-1.0.3/email_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-25 19:58:09.000000 easy-email-builder-1.0.3/email_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 19:58:09.000000 easy-email-builder-1.0.3/email_builder/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:58:19.413206 easy-email-builder-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 19:58:09.000000 easy-email-builder-1.0.3/setup.py
```

### Comparing `easy-email-builder-1.0.2/PKG-INFO` & `easy-email-builder-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-email-builder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple interface for sending emails with the builder design pattern with different services.
 Author: Ryan Schreiber
 Author-email: ryanschreiber86@gmail.com
 Project-URL: Documentation, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Source, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Tracker, https://github.com/ryan-schreiber/email-builder/issues
 Keywords: email emails builder smtp gmail ses aws
@@ -84,15 +84,15 @@
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
     .subject("test email sent from my python lib")
-    .html("<h1> hello world </h1>")
+    .markdown("# hello world")
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
 ).send(email_builder.clients.SES())
 ```
 
 ## Email Options
 
@@ -136,18 +136,21 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # you need to choose between either html or text, can't use both
+    # you need to choose between either html, markdown or text, can't use more than one
 
-    # html(body:str) -> renders the given html in the email body, no chaining
+    # html(data:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
+	
+	# markdown(body:str) -> renders the given markdown as html in the email body, no chaining
+    .markdown("# hello world")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
     # attachment(attachment:email_builder.Attchment) -> chain as many of these as you want
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
```

### Comparing `easy-email-builder-1.0.2/README.md` & `easy-email-builder-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
     .subject("test email sent from my python lib")
-    .html("<h1> hello world </h1>")
+    .markdown("# hello world")
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
 ).send(email_builder.clients.SES())
 ```
 
 ## Email Options
 
@@ -121,18 +121,21 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # you need to choose between either html or text, can't use both
+    # you need to choose between either html, markdown or text, can't use more than one
 
-    # html(body:str) -> renders the given html in the email body, no chaining
+    # html(data:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
+	
+	# markdown(body:str) -> renders the given markdown as html in the email body, no chaining
+    .markdown("# hello world")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
     # attachment(attachment:email_builder.Attchment) -> chain as many of these as you want
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
```

### Comparing `easy-email-builder-1.0.2/easy_email_builder.egg-info/PKG-INFO` & `easy-email-builder-1.0.3/easy_email_builder.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easy-email-builder
-Version: 1.0.2
+Version: 1.0.3
 Summary: Simple interface for sending emails with the builder design pattern with different services.
 Author: Ryan Schreiber
 Author-email: ryanschreiber86@gmail.com
 Project-URL: Documentation, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Source, https://github.com/ryan-schreiber/email-builder/
 Project-URL: Tracker, https://github.com/ryan-schreiber/email-builder/issues
 Keywords: email emails builder smtp gmail ses aws
@@ -84,15 +84,15 @@
 client = email_builder.clients.SES()
 email = (
   email_builder.Email()
     .sender("my.email@company.com")
     .to("recipient.1@company.com")
     .to("recipient.2@company.com")
     .subject("test email sent from my python lib")
-    .html("<h1> hello world </h1>")
+    .markdown("# hello world")
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
 ).send(email_builder.clients.SES())
 ```
 
 ## Email Options
 
@@ -136,18 +136,21 @@
     .bcc("recipient.1@company.com")
     .bcc("recipient.2@company.com")
 
     # subject(subject:str) -> only one subject line allowed
     .subject("test email sent from my python lib")
 
     # --- EMAIL BODY --- #
-    # you need to choose between either html or text, can't use both
+    # you need to choose between either html, markdown or text, can't use more than one
 
-    # html(body:str) -> renders the given html in the email body, no chaining
+    # html(data:str) -> renders the given html in the email body, no chaining
     .html("<h1> hello world </h1>")
+	
+	# markdown(body:str) -> renders the given markdown as html in the email body, no chaining
+    .markdown("# hello world")
 
     # test(body:str) -> adds the given text to the email body as plain text
     .text("hello world")
 
     # attachment(attachment:email_builder.Attchment) -> chain as many of these as you want
     .attachment(email_builder.Attachment("report.csv", data))
     .attachment(email_builder.Attachment("test2.json", """{"key": "value"}"""))
```

### Comparing `easy-email-builder-1.0.2/email_builder/__init__.py` & `easy-email-builder-1.0.3/email_builder/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 
 from email.mime.multipart import MIMEMultipart
 from email.mime.base import MIMEBase
 from email.mime.text import MIMEText
 from email.mime.application import MIMEApplication
 from copy import deepcopy
+import markdown
 
 import email_builder.clients
 
 class Email:
 
   def __init__(self):
     self.__message = MIMEMultipart('mixed')
@@ -51,14 +52,19 @@
   def subject(self, subject):
     self.__message["Subject"] = subject
     return self
   
   def html(self, data):
     self.__body.attach(MIMEText(data.encode(self.__charset), 'html', self.__charset))
     return self
+    
+  def markdown(self, data):
+    data = markdown.markdown(data)
+    self.__body.attach(MIMEText(data.encode(self.__charset), 'html', self.__charset))
+    return self
   
   def text(self, data):
     self.__body.attach(MIMEText(data.encode(self.__charset), 'plain', self.__charset))
     return self
   
   def attachment(self, *attachments):
     for attachment in attachments:
```

### Comparing `easy-email-builder-1.0.2/email_builder/clients.py` & `easy-email-builder-1.0.3/email_builder/clients.py`

 * *Files identical despite different names*

### Comparing `easy-email-builder-1.0.2/setup.py` & `easy-email-builder-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().split("\n")
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='easy-email-builder',
-    version='1.0.2',
+    version='1.0.3',
     description='Simple interface for sending emails with the builder design pattern with different services.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ryan Schreiber',
     author_email='ryanschreiber86@gmail.com',
     packages=find_packages(),
     install_requires=requirements,
```

