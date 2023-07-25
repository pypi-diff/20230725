# Comparing `tmp/easy-email-builder-1.0.tar.gz` & `tmp/easy-email-builder-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy-email-builder-1.0.tar", last modified: Tue Jul 25 18:57:17 2023, max compression
+gzip compressed data, was "easy-email-builder-1.0.1.tar", last modified: Tue Jul 25 19:28:07 2023, max compression
```

## Comparing `easy-email-builder-1.0.tar` & `easy-email-builder-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:57:17.326546 easy-email-builder-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 18:57:17.326546 easy-email-builder-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 18:57:06.000000 easy-email-builder-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:57:17.326546 easy-email-builder-1.0/easy_email_builder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 18:57:17.000000 easy-email-builder-1.0/easy_email_builder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 18:57:17.000000 easy-email-builder-1.0/easy_email_builder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:57:17.000000 easy-email-builder-1.0/easy_email_builder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 18:57:17.000000 easy-email-builder-1.0/easy_email_builder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 18:57:17.000000 easy-email-builder-1.0/easy_email_builder.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:57:17.326546 easy-email-builder-1.0/email_builder/
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 18:57:06.000000 easy-email-builder-1.0/email_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 18:57:06.000000 easy-email-builder-1.0/email_builder/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:57:17.326546 easy-email-builder-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-25 18:57:06.000000 easy-email-builder-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4067 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/easy_email_builder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 19:28:07.000000 easy-email-builder-1.0.1/easy_email_builder.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/email_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/email_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/email_builder/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 19:28:07.325830 easy-email-builder-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-25 19:27:58.000000 easy-email-builder-1.0.1/setup.py
```

### Comparing `easy-email-builder-1.0/email_builder/__init__.py` & `easy-email-builder-1.0.1/email_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `easy-email-builder-1.0/email_builder/clients.py` & `easy-email-builder-1.0.1/email_builder/clients.py`

 * *Files identical despite different names*

### Comparing `easy-email-builder-1.0/setup.py` & `easy-email-builder-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().split("\n")
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='easy-email-builder',
-    version='1.0',
+    version='1.0.1',
     description='Simple interface for sending emails with the builder design pattern with different services.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ryan Schreiber',
     author_email='ryanschreiber86@gmail.com',
     packages=find_packages(),
     install_requires=requirements,
```

