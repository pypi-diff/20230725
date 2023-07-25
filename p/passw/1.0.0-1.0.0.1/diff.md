# Comparing `tmp/passw-1.0.0.tar.gz` & `tmp/passw-1.0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passw-1.0.0.tar", last modified: Tue Jul 25 10:55:52 2023, max compression
+gzip compressed data, was "passw-1.0.0.1.tar", last modified: Tue Jul 25 11:02:35 2023, max compression
```

## Comparing `passw-1.0.0.tar` & `passw-1.0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:55:52.987485 passw-1.0.0/
--rw-rw-r--   0 user      (1000) user      (1000)      255 2023-07-25 10:55:52.987485 passw-1.0.0/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:55:52.987485 passw-1.0.0/passw/
--rw-rw-r--   0 user      (1000) user      (1000)       52 2023-07-25 10:51:31.000000 passw-1.0.0/passw/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      654 2023-07-25 10:54:54.000000 passw-1.0.0/passw/generate_pass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 10:55:52.987485 passw-1.0.0/passw.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      255 2023-07-25 10:55:52.000000 passw-1.0.0/passw.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      165 2023-07-25 10:55:52.000000 passw-1.0.0/passw.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 10:55:52.000000 passw-1.0.0/passw.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-25 10:55:52.000000 passw-1.0.0/passw.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 10:55:52.987485 passw-1.0.0/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      383 2023-07-25 10:53:35.000000 passw-1.0.0/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:02:35.120911 passw-1.0.0.1/
+-rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:02:35.120911 passw-1.0.0.1/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:02:35.120911 passw-1.0.0.1/passw/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-07-25 11:01:52.000000 passw-1.0.0.1/passw/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      773 2023-07-25 11:01:59.000000 passw-1.0.0.1/passw/generate_pass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:02:35.120911 passw-1.0.0.1/passw.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:02:35.000000 passw-1.0.0.1/passw.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      165 2023-07-25 11:02:35.000000 passw-1.0.0.1/passw.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 11:02:35.000000 passw-1.0.0.1/passw.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-25 11:02:35.000000 passw-1.0.0.1/passw.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:02:35.120911 passw-1.0.0.1/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-25 11:02:11.000000 passw-1.0.0.1/setup.py
```

### Comparing `passw-1.0.0/passw/generate_pass.py` & `passw-1.0.0.1/passw/generate_pass.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,8 +15,12 @@
             any(c.isupper() for c in password) and
             any(c.isdigit() for c in password)):
             break
 
     return password
 
 
-
+def gen_pass():
+    paas_len = random.randInt(6,12)
+    passw = generate_random_password(pass_len)
+    return passw
+
```

