# Comparing `tmp/quickbeutils-1.2.1.tar.gz` & `tmp/quickbeutils-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickbeutils-1.2.1.tar", last modified: Thu Sep 15 04:15:23 2022, max compression
+gzip compressed data, was "quickbeutils-1.2.2.tar", last modified: Tue Jul 25 11:25:10 2023, max compression
```

## Comparing `quickbeutils-1.2.1.tar` & `quickbeutils-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 04:15:23.633634 quickbeutils-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-15 04:15:23.633634 quickbeutils-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 04:15:23.633634 quickbeutils-1.2.1/quickbeutils/
--rw-r--r--   0 runner    (1001) docker     (121)     7968 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/quickbeutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/quickbeutils/aws_ses.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/quickbeutils/gmail.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/quickbeutils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/quickbeutils/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-15 04:15:23.633634 quickbeutils-1.2.1/quickbeutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-15 04:15:23.000000 quickbeutils-1.2.1/quickbeutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      314 2022-09-15 04:15:23.000000 quickbeutils-1.2.1/quickbeutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-15 04:15:23.000000 quickbeutils-1.2.1/quickbeutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-09-15 04:15:23.000000 quickbeutils-1.2.1/quickbeutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-15 04:15:23.000000 quickbeutils-1.2.1/quickbeutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-15 04:15:23.633634 quickbeutils-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-09-15 04:15:13.000000 quickbeutils-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/quickbeutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8471 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/quickbeutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/quickbeutils/aws_ses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/quickbeutils/gmail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/quickbeutils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/quickbeutils/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/quickbeutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-25 11:25:10.000000 quickbeutils-1.2.2/quickbeutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-25 11:25:10.000000 quickbeutils-1.2.2/quickbeutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 11:25:10.000000 quickbeutils-1.2.2/quickbeutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 11:25:10.000000 quickbeutils-1.2.2/quickbeutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 11:25:10.000000 quickbeutils-1.2.2/quickbeutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 11:25:10.520397 quickbeutils-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/tests/test_send_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/tests/test_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/tests/test_srting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-25 11:24:56.000000 quickbeutils-1.2.2/tests/test_utils.py
```

### Comparing `quickbeutils-1.2.1/PKG-INFO` & `quickbeutils-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbeutils
-Version: 1.2.1
+Version: 1.2.2
 Summary: All sorts of utilities
 Home-page: https://github.com/eldad1221/quickbelog
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickbeutils-1.2.1/quickbeutils/__init__.py` & `quickbeutils-1.2.2/quickbeutils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,44 @@
 import os
 import json
+import base64
 import random
 from time import sleep
 from datetime import timedelta, datetime
 from quickbelog import Log
 import quickbeutils.gmail as gmail
 import quickbeutils.aws_ses as aws_ses
 import quickbeutils.slack as slack
 from email.utils import formataddr
 from smtplib import SMTPException
 from email.mime.text import MIMEText
 from email.mime.multipart import MIMEMultipart
+from email.mime.application import MIMEApplication
 
 SEND_EMAIL_VIA_GMAIL = 'GMAIL'
 SEND_EMAIL_VIA_SMTP = 'SMTP'
 SEND_EMAIL_VIA_AWS_SES = 'AWS_SES'
 
 
 def send_email(
         sender: str, recipient: str,
         subject: str = None, sender_name: str = None,
         body_text: str = '',
         body_html: str = None,
+        attachments: dict = None,
         send_via: str = SEND_EMAIL_VIA_SMTP) -> bool:
     """
 
     :param body_html:
     :param body_text:
     :param sender: "From" address
+    :param sender_name: Sender name is optional.
     :param recipient: "To" address.
     :param subject: The subject line of the email.
-    :param sender_name: Sender name is optional.
+    :param attachments: Dictionary of base64 strings for attached files, file name as dictionary key
     :param send_via: One of the following: SMTP, AWS_SES, GMAIL
     :return:
     """
 
     # Create message container - the correct MIME type is multipart/alternative.
     msg = MIMEMultipart('alternative')
     msg['Subject'] = subject
@@ -46,14 +50,20 @@
         body_html = f"<html><head><title>{subject}</title></head><body>{txt}</body></html>"
 
     # Record the MIME types of both parts - text/plain and text/html
     # According to RFC 2046, the last part of a multipart message, in this case the HTML message is preferred.
     msg.attach(MIMEText(body_text, 'plain'))
     msg.attach(MIMEText(body_html, 'html'))
 
+    if attachments is not None:
+        for f_name, f_base64 in attachments.items():
+            attachment = MIMEApplication(base64.b64decode(f_base64.encode()), _subtype="txt")
+            attachment.add_header('Content-Disposition', 'attachment', filename=f_name)
+            msg.attach(attachment)
+
     send_via = send_via.upper().strip()
 
     try:
         if send_via == SEND_EMAIL_VIA_AWS_SES:
             aws_ses.send(sender=sender, recipient=recipient, msg=msg)
         elif send_via == SEND_EMAIL_VIA_GMAIL:
             gmail.send(sender=sender, recipient=recipient, msg=msg)
```

### Comparing `quickbeutils-1.2.1/quickbeutils/aws_ses.py` & `quickbeutils-1.2.2/quickbeutils/aws_ses.py`

 * *Files identical despite different names*

### Comparing `quickbeutils-1.2.1/quickbeutils/gmail.py` & `quickbeutils-1.2.2/quickbeutils/gmail.py`

 * *Files identical despite different names*

### Comparing `quickbeutils-1.2.1/quickbeutils/slack.py` & `quickbeutils-1.2.2/quickbeutils/slack.py`

 * *Files identical despite different names*

### Comparing `quickbeutils-1.2.1/quickbeutils.egg-info/PKG-INFO` & `quickbeutils-1.2.2/quickbeutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickbeutils
-Version: 1.2.1
+Version: 1.2.2
 Summary: All sorts of utilities
 Home-page: https://github.com/eldad1221/quickbelog
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickbeutils-1.2.1/setup.py` & `quickbeutils-1.2.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="quickbeutils",
-    version="1.2.1",
+    version="1.2.2",
     author="Eldad Bishari",
     author_email="eldad@1221tlv.org",
     description="All sorts of utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eldad1221/quickbelog",
     packages=setuptools.find_packages(),
```

