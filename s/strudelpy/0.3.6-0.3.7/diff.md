# Comparing `tmp/strudelpy-0.3.6.tar.gz` & `tmp/strudelpy-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/strudelpy-0.3.6.tar", last modified: Thu Jul 11 11:21:54 2019, max compression
+gzip compressed data, was "strudelpy-0.3.7.tar", last modified: Tue Jul 25 00:36:53 2023, max compression
```

## Comparing `strudelpy-0.3.6.tar` & `strudelpy-0.3.7.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 harel     (1000) harel     (1000)        0 2019-07-11 11:21:54.000000 strudelpy-0.3.6/
--rw-r--r--   0 harel     (1000) harel     (1000)      839 2019-07-11 11:21:54.000000 strudelpy-0.3.6/PKG-INFO
-drwxr-xr-x   0 harel     (1000) harel     (1000)        0 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy/
--rw-r--r--   0 harel     (1000) harel     (1000)    12916 2019-07-11 11:21:12.000000 strudelpy-0.3.6/strudelpy/__init__.py
-drwxr-xr-x   0 harel     (1000) harel     (1000)        0 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy/tests/
--rw-r--r--   0 harel     (1000) harel     (1000)     9572 2019-01-28 00:01:35.000000 strudelpy-0.3.6/strudelpy/tests/tests.py
--rw-r--r--   0 harel     (1000) harel     (1000)        0 2019-01-28 00:01:35.000000 strudelpy-0.3.6/strudelpy/tests/__init__.py
--rw-r--r--   0 harel     (1000) harel     (1000)       79 2019-07-11 11:21:54.000000 strudelpy-0.3.6/setup.cfg
--rw-r--r--   0 harel     (1000) harel     (1000)     3155 2019-07-11 11:21:25.000000 strudelpy-0.3.6/README.md
--rw-r--r--   0 harel     (1000) harel     (1000)     1109 2019-07-11 11:21:32.000000 strudelpy-0.3.6/setup.py
-drwxr-xr-x   0 harel     (1000) harel     (1000)        0 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/
--rw-r--r--   0 harel     (1000) harel     (1000)      839 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/PKG-INFO
--rw-r--r--   0 harel     (1000) harel     (1000)        4 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/requires.txt
--rw-r--r--   0 harel     (1000) harel     (1000)      267 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/SOURCES.txt
--rw-r--r--   0 harel     (1000) harel     (1000)        1 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/dependency_links.txt
--rw-r--r--   0 harel     (1000) harel     (1000)       10 2019-07-11 11:21:54.000000 strudelpy-0.3.6/strudelpy.egg-info/top_level.txt
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/
+-rw-rw-r--   0 harel     (1000) harel     (1000)     1077 2023-07-24 23:27:58.000000 strudelpy-0.3.7/LICENSE.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-25 00:36:53.199488 strudelpy-0.3.7/PKG-INFO
+-rw-rw-r--   0 harel     (1000) harel     (1000)     3155 2023-07-25 00:34:08.000000 strudelpy-0.3.7/README.md
+-rw-rw-r--   0 harel     (1000) harel     (1000)       79 2023-07-25 00:36:53.199488 strudelpy-0.3.7/setup.cfg
+-rw-rw-r--   0 harel     (1000) harel     (1000)     1094 2023-07-25 00:33:57.000000 strudelpy-0.3.7/setup.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.195488 strudelpy-0.3.7/strudelpy/
+-rw-rw-r--   0 harel     (1000) harel     (1000)    12923 2023-07-25 00:33:18.000000 strudelpy-0.3.7/strudelpy/__init__.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/strudelpy/tests/
+-rw-rw-r--   0 harel     (1000) harel     (1000)        0 2023-07-24 23:27:58.000000 strudelpy-0.3.7/strudelpy/tests/__init__.py
+-rw-rw-r--   0 harel     (1000) harel     (1000)     9572 2023-07-24 23:27:58.000000 strudelpy-0.3.7/strudelpy/tests/tests.py
+drwxrwxr-x   0 harel     (1000) harel     (1000)        0 2023-07-25 00:36:53.199488 strudelpy-0.3.7/strudelpy.egg-info/
+-rw-rw-r--   0 harel     (1000) harel     (1000)      854 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/PKG-INFO
+-rw-rw-r--   0 harel     (1000) harel     (1000)      279 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)        1 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)        4 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/requires.txt
+-rw-rw-r--   0 harel     (1000) harel     (1000)       10 2023-07-25 00:36:53.000000 strudelpy-0.3.7/strudelpy.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `strudelpy-0.3.6/PKG-INFO` & `strudelpy-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: strudelpy
-Version: 0.3.6
+Version: 0.3.7
 Summary: Easy as Pie Emails in Python
 Home-page: https://github.com/harel/strudelpy
 Author: Harel Malka
 Author-email: harel@harelmalka.com
 License: MIT
 Download-URL: https://github.com/harel/strudelpy/archive/0.3.tar.gz
-Description: StrudelPy is an easy to use library to manage sending emails in a OO way.The library is comprised of a SMTP object to manage connections to SMTPservers and an Email object to handle the messages themselves.Supports Python 2 and 3.
 Keywords: email,smtp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Email
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE.txt
+
+StrudelPy is an easy to use library to manage sending emails in a OO way.The library is comprised of a SMTP object to manage connections to SMTPservers and an Email object to handle the messages themselves.Supports Python 2 and 3.
+
```

### Comparing `strudelpy-0.3.6/strudelpy/__init__.py` & `strudelpy-0.3.7/strudelpy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from email.mime.multipart import MIMEMultipart
 from email.header import Header
 from email.utils import formatdate, formataddr, make_msgid
 from email.encoders import encode_base64
 from email.charset import Charset
 
 __author__ = 'Harel Malka'
-__version__ = '0.3.6'
+__version__ = '0.3.7'
 
 # initialise the mimetypes module
 mimetypes.init()
 
 try:
     PROTOCOL_TLS = getattr(ssl, os.environ.get('EMAIL_TLS_VERSION', 'PROTOCOL_TLSv1_2'))
 except AttributeError:
@@ -107,15 +107,15 @@
         if self.username and self.password:
             try:
                 self.client.login(six.u(self.username), six.u(self.password))
             except (smtplib.SMTPException, smtplib.SMTPAuthenticationError):
                 # if login fails, try again using a manual plain login method
                 self.client.connect(host=self.host, port=self.port)
                 self.client.docmd("AUTH LOGIN", base64.b64encode(six.b(self.username)))
-                self.client.docmd(base64.b64encode(six.b(self.password)), "")
+                self.client.docmd(base64.b64encode(six.b(self.password)), six.b(""))
         else:
             self.client.connect()
 
     def close(self):
         self.client.quit()
 
     def send(self, email):
```

### Comparing `strudelpy-0.3.6/strudelpy/tests/tests.py` & `strudelpy-0.3.7/strudelpy/tests/tests.py`

 * *Files identical despite different names*

### Comparing `strudelpy-0.3.6/README.md` & `strudelpy-0.3.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## StrudelPy v0.3.6
+## StrudelPy v0.3.7
 ### A tastier way to send emails with Python
 
 ### Features
 * Attachments, multiple recipients, cc, bcc - the standard stuff
 * Embedded Images
 * Plays well with Unicode
 * Easy OOP approach
```

### Comparing `strudelpy-0.3.6/setup.py` & `strudelpy-0.3.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup
 
 setup(
-    name = 'strudelpy',
-    version = '0.3.6',
-    description = 'Easy as Pie Emails in Python',
+    name='strudelpy',
+    version='0.3.7',
+    description='Easy as Pie Emails in Python',
     long_description='StrudelPy is an easy to use library to manage sending emails in a OO way.'
                      'The library is comprised of a SMTP object to manage connections to SMTP'
                      'servers and an Email object to handle the messages themselves.'
                      'Supports Python 2 and 3.',
-    author = 'Harel Malka',
-    author_email = 'harel@harelmalka.com',
-    url = 'https://github.com/harel/strudelpy',
-    download_url = 'https://github.com/harel/strudelpy/archive/0.3.tar.gz',
-    keywords = ['email', 'smtp'], # arbitrary keywords
+    author='Harel Malka',
+    author_email='harel@harelmalka.com',
+    url='https://github.com/harel/strudelpy',
+    download_url='https://github.com/harel/strudelpy/archive/0.3.tar.gz',
+    keywords=['email', 'smtp'],  # arbitrary keywords
     install_requires=['six'],
     license='MIT',
     packages=['strudelpy', 'strudelpy.tests'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'License :: OSI Approved :: MIT License',
         'Intended Audience :: Developers',
```

### Comparing `strudelpy-0.3.6/strudelpy.egg-info/PKG-INFO` & `strudelpy-0.3.7/strudelpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: strudelpy
-Version: 0.3.6
+Version: 0.3.7
 Summary: Easy as Pie Emails in Python
 Home-page: https://github.com/harel/strudelpy
 Author: Harel Malka
 Author-email: harel@harelmalka.com
 License: MIT
 Download-URL: https://github.com/harel/strudelpy/archive/0.3.tar.gz
-Description: StrudelPy is an easy to use library to manage sending emails in a OO way.The library is comprised of a SMTP object to manage connections to SMTPservers and an Email object to handle the messages themselves.Supports Python 2 and 3.
 Keywords: email,smtp
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Communications :: Email
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
+License-File: LICENSE.txt
+
+StrudelPy is an easy to use library to manage sending emails in a OO way.The library is comprised of a SMTP object to manage connections to SMTPservers and an Email object to handle the messages themselves.Supports Python 2 and 3.
+
```

