# Comparing `tmp/pwdsphinx-1.0rc4.tar.gz` & `tmp/pwdsphinx-1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdsphinx-1.0rc4.tar", last modified: Fri Jul 16 18:10:50 2021, max compression
+gzip compressed data, was "pwdsphinx-1.0rc5.tar", last modified: Fri Jul 16 20:06:13 2021, max compression
```

## Comparing `pwdsphinx-1.0rc4.tar` & `pwdsphinx-1.0rc5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 18:10:50.378944 pwdsphinx-1.0rc4/
--rw-r--r--   0 s         (1000) s         (1000)       31 2018-03-05 13:15:42.000000 pwdsphinx-1.0rc4/MANIFEST.in
--rw-r--r--   0 s         (1000) s         (1000)    12136 2021-07-16 18:10:50.378944 pwdsphinx-1.0rc4/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)     9448 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc4/README.md
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 18:10:50.378944 pwdsphinx-1.0rc4/pwdsphinx/
--rw-r--r--   0 s         (1000) s         (1000)        0 2018-03-05 13:15:42.000000 pwdsphinx-1.0rc4/pwdsphinx/__init__.py
--rwxr-xr-x   0 s         (1000) s         (1000)     2514 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc4/pwdsphinx/bin2pass.py
--rwxr-xr-x   0 s         (1000) s         (1000)      837 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc4/pwdsphinx/config.py
--rwxr-xr-x   0 s         (1000) s         (1000)    15844 2021-07-16 17:55:32.000000 pwdsphinx-1.0rc4/pwdsphinx/oracle.py
--rwxr-xr-x   0 s         (1000) s         (1000)     3882 2021-05-11 00:41:49.000000 pwdsphinx-1.0rc4/pwdsphinx/rules.py
--rwxr-xr-x   0 s         (1000) s         (1000)    20988 2021-07-16 17:06:39.000000 pwdsphinx-1.0rc4/pwdsphinx/sphinx.py
--rwxr-xr-x   0 s         (1000) s         (1000)     2781 2021-01-15 22:44:13.000000 pwdsphinx-1.0rc4/pwdsphinx/sphinxlib.py
--rwxr-xr-x   0 s         (1000) s         (1000)     6975 2021-04-26 00:09:43.000000 pwdsphinx-1.0rc4/pwdsphinx/websphinx.py
-drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 18:10:50.378944 pwdsphinx-1.0rc4/pwdsphinx.egg-info/
--rw-r--r--   0 s         (1000) s         (1000)    12136 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/PKG-INFO
--rw-r--r--   0 s         (1000) s         (1000)      399 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/SOURCES.txt
--rw-r--r--   0 s         (1000) s         (1000)        1 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/dependency_links.txt
--rw-r--r--   0 s         (1000) s         (1000)      153 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/entry_points.txt
--rw-r--r--   0 s         (1000) s         (1000)       57 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/requires.txt
--rw-r--r--   0 s         (1000) s         (1000)       10 2021-07-16 18:10:50.000000 pwdsphinx-1.0rc4/pwdsphinx.egg-info/top_level.txt
--rw-r--r--   0 s         (1000) s         (1000)       38 2021-07-16 18:10:50.382278 pwdsphinx-1.0rc4/setup.cfg
--rwxr-xr-x   0 s         (1000) s         (1000)     1603 2021-07-16 18:07:57.000000 pwdsphinx-1.0rc4/setup.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 20:06:13.309260 pwdsphinx-1.0rc5/
+-rw-r--r--   0 s         (1000) s         (1000)       31 2018-03-05 13:15:42.000000 pwdsphinx-1.0rc5/MANIFEST.in
+-rw-r--r--   0 s         (1000) s         (1000)    12136 2021-07-16 20:06:13.309260 pwdsphinx-1.0rc5/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)     9448 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc5/README.md
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 20:06:13.309260 pwdsphinx-1.0rc5/pwdsphinx/
+-rw-r--r--   0 s         (1000) s         (1000)        0 2018-03-05 13:15:42.000000 pwdsphinx-1.0rc5/pwdsphinx/__init__.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     2514 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc5/pwdsphinx/bin2pass.py
+-rwxr-xr-x   0 s         (1000) s         (1000)      837 2021-06-29 16:34:01.000000 pwdsphinx-1.0rc5/pwdsphinx/config.py
+-rwxr-xr-x   0 s         (1000) s         (1000)    15844 2021-07-16 17:55:32.000000 pwdsphinx-1.0rc5/pwdsphinx/oracle.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     3882 2021-05-11 00:41:49.000000 pwdsphinx-1.0rc5/pwdsphinx/rules.py
+-rwxr-xr-x   0 s         (1000) s         (1000)    21071 2021-07-16 19:57:39.000000 pwdsphinx-1.0rc5/pwdsphinx/sphinx.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     2781 2021-01-15 22:44:13.000000 pwdsphinx-1.0rc5/pwdsphinx/sphinxlib.py
+-rwxr-xr-x   0 s         (1000) s         (1000)     6975 2021-04-26 00:09:43.000000 pwdsphinx-1.0rc5/pwdsphinx/websphinx.py
+drwxr-xr-x   0 s         (1000) s         (1000)        0 2021-07-16 20:06:13.309260 pwdsphinx-1.0rc5/pwdsphinx.egg-info/
+-rw-r--r--   0 s         (1000) s         (1000)    12136 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/PKG-INFO
+-rw-r--r--   0 s         (1000) s         (1000)      399 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/SOURCES.txt
+-rw-r--r--   0 s         (1000) s         (1000)        1 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/dependency_links.txt
+-rw-r--r--   0 s         (1000) s         (1000)      153 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/entry_points.txt
+-rw-r--r--   0 s         (1000) s         (1000)       57 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/requires.txt
+-rw-r--r--   0 s         (1000) s         (1000)       10 2021-07-16 20:06:13.000000 pwdsphinx-1.0rc5/pwdsphinx.egg-info/top_level.txt
+-rw-r--r--   0 s         (1000) s         (1000)       38 2021-07-16 20:06:13.309260 pwdsphinx-1.0rc5/setup.cfg
+-rwxr-xr-x   0 s         (1000) s         (1000)     1603 2021-07-16 20:05:43.000000 pwdsphinx-1.0rc5/setup.py
```

### Comparing `pwdsphinx-1.0rc4/PKG-INFO` & `pwdsphinx-1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdsphinx
-Version: 1.0rc4
+Version: 1.0rc5
 Summary: SPHINX password protocol
 Home-page: https://github.com/stef/pwdsphinx
 Author: Stefan Marsiske
 Author-email: sphinx@ctrlc.hu
 License: GPLv3
 Description: <!--
         SPDX-FileCopyrightText: 2018, Marsiske Stefan
```

### Comparing `pwdsphinx-1.0rc4/README.md` & `pwdsphinx-1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/bin2pass.py` & `pwdsphinx-1.0rc5/pwdsphinx/bin2pass.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/config.py` & `pwdsphinx-1.0rc5/pwdsphinx/config.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/oracle.py` & `pwdsphinx-1.0rc5/pwdsphinx/oracle.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/rules.py` & `pwdsphinx-1.0rc5/pwdsphinx/rules.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/sphinx.py` & `pwdsphinx-1.0rc5/pwdsphinx/sphinx.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,16 @@
 
 ENC_CTX = b"sphinx encryption key"
 SIGN_CTX = b"sphinx signing key"
 SALT_CTX = b"sphinx host salt"
 PASS_CTX = b"sphinx password context"
 CHECK_CTX = b"sphinx check digit context"
 
+VERSION = b'\x00'
+
 RULE_SIZE = 79
 
 #### Helper fns ####
 
 def get_masterkey():
   try:
     with open(os.path.join(datadir,'masterkey'), 'rb') as fd:
@@ -113,28 +115,28 @@
   clearmem(mk)
   return sk
 
 def encrypt_blob(blob):
   # todo implement padding
   sk = get_sealkey()
   nonce = pysodium.randombytes(pysodium.crypto_secretbox_NONCEBYTES)
-  ct = pysodium.crypto_secretbox(blob,nonce,sk)
+  ct = pysodium.crypto_aead_xchacha20poly1305_ietf_encrypt(blob,VERSION,nonce,sk)
   clearmem(sk)
-  return b'\x00'+nonce+ct
+  return VERSION+nonce+ct
 
 def decrypt_blob(blob):
   # todo implement padding
   sk = get_sealkey()
-  version = blob[0]
+  version = blob[:1]
   blob = blob[1:]
   nonce = blob[:pysodium.crypto_secretbox_NONCEBYTES]
   blob = blob[pysodium.crypto_secretbox_NONCEBYTES:]
-  res = pysodium.crypto_secretbox_open(blob,nonce,sk)
+  res = pysodium.crypto_aead_xchacha20poly1305_ietf_decrypt(blob,version,nonce,sk)
   clearmem(sk)
-  return version, res
+  return VERSION, res
 
 def sign_blob(blob, id, rwd):
   sk, pk = get_signkey(id, rwd)
   res = pysodium.crypto_sign_detached(blob,sk)
   clearmem(sk)
   return b''.join((blob,res))
```

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/sphinxlib.py` & `pwdsphinx-1.0rc5/pwdsphinx/sphinxlib.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx/websphinx.py` & `pwdsphinx-1.0rc5/pwdsphinx/websphinx.py`

 * *Files identical despite different names*

### Comparing `pwdsphinx-1.0rc4/pwdsphinx.egg-info/PKG-INFO` & `pwdsphinx-1.0rc5/pwdsphinx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pwdsphinx
-Version: 1.0rc4
+Version: 1.0rc5
 Summary: SPHINX password protocol
 Home-page: https://github.com/stef/pwdsphinx
 Author: Stefan Marsiske
 Author-email: sphinx@ctrlc.hu
 License: GPLv3
 Description: <!--
         SPDX-FileCopyrightText: 2018, Marsiske Stefan
```

### Comparing `pwdsphinx-1.0rc4/setup.py` & `pwdsphinx-1.0rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Used for the long_description.  It's nice, because now 1) we have a top level
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(name = 'pwdsphinx',
-       version = '1.0-rc4',
+       version = '1.0-rc5',
        description = 'SPHINX password protocol',
        license = "GPLv3",
        author = 'Stefan Marsiske',
        author_email = 'sphinx@ctrlc.hu',
        url = 'https://github.com/stef/pwdsphinx',
        long_description=read('README.md'),
        long_description_content_type="text/markdown",
```

