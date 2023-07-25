# Comparing `tmp/passw-1.0.0.2.tar.gz` & `tmp/passw-1.0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "passw-1.0.0.2.tar", last modified: Tue Jul 25 11:04:50 2023, max compression
+gzip compressed data, was "passw-1.0.0.3.tar", last modified: Tue Jul 25 11:06:35 2023, max compression
```

## Comparing `passw-1.0.0.2.tar` & `passw-1.0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:04:50.786788 passw-1.0.0.2/
--rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:04:50.786788 passw-1.0.0.2/PKG-INFO
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:04:50.786788 passw-1.0.0.2/passw/
--rw-rw-r--   0 user      (1000) user      (1000)       36 2023-07-25 11:01:52.000000 passw-1.0.0.2/passw/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      773 2023-07-25 11:04:14.000000 passw-1.0.0.2/passw/generate_pass.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:04:50.786788 passw-1.0.0.2/passw.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:04:50.000000 passw-1.0.0.2/passw.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      165 2023-07-25 11:04:50.000000 passw-1.0.0.2/passw.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 11:04:50.000000 passw-1.0.0.2/passw.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-25 11:04:50.000000 passw-1.0.0.2/passw.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:04:50.786788 passw-1.0.0.2/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-25 11:04:22.000000 passw-1.0.0.2/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/
+-rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:06:35.332245 passw-1.0.0.3/PKG-INFO
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/passw/
+-rw-rw-r--   0 user      (1000) user      (1000)       36 2023-07-25 11:01:52.000000 passw-1.0.0.3/passw/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      773 2023-07-25 11:06:21.000000 passw-1.0.0.3/passw/generate_pass.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-07-25 11:06:35.332245 passw-1.0.0.3/passw.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)      257 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      165 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        6 2023-07-25 11:06:35.000000 passw-1.0.0.3/passw.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-07-25 11:06:35.332245 passw-1.0.0.3/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)      385 2023-07-25 11:06:29.000000 passw-1.0.0.3/setup.py
```

### Comparing `passw-1.0.0.2/passw/generate_pass.py` & `passw-1.0.0.3/passw/generate_pass.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,11 +16,11 @@
             any(c.isdigit() for c in password)):
             break
 
     return password
 
 
 def gen_pass():
-    paas_len = random.randint(6,12)
+    pass_len = random.randint(6,12)
     passw = generate_random_password(pass_len)
     return passw
```

