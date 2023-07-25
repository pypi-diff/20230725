# Comparing `tmp/salure_helpers_ftp-1.5.4.tar.gz` & `tmp/salure_helpers_ftp-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.5.4.tar", last modified: Tue Jul 25 09:57:11 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.5.5.tar", last modified: Tue Jul 25 10:08:54 2023, max compression
```

## Comparing `salure_helpers_ftp-1.5.4.tar` & `salure_helpers_ftp-1.5.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/
--rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-25 10:08:34.000000 salure_helpers_ftp-1.5.5/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2023-07-25 10:08:34.000000 salure_helpers_ftp-1.5.5/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6340 2023-07-25 10:08:34.000000 salure_helpers_ftp-1.5.5/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 10:08:54.000000 salure_helpers_ftp-1.5.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-25 10:08:34.000000 salure_helpers_ftp-1.5.5/setup.py
```

### Comparing `salure_helpers_ftp-1.5.4/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.5.5/salure_helpers/ftp/ftps.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_ftp-1.5.4/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.5.5/salure_helpers/ftp/sftp.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.username = credentials['username']
         self.password = credentials['password']
         self.cnopts = pysftp.CnOpts()
         self.cnopts.hostkeys = None
         self.private_key_path = None
         if credentials['private_key_path'] is not None:
             self.private_key_path = credentials['private_key_path']
-            self.private_key_password = credentials['private_key_password']
+            self.private_key_pass = credentials['private_key_password']
 
     def upload_file(self, local_filepath, remote_filepath, confirm=True) -> SFTPAttributes:
         """
         Upload a single file to a remote location. If there is no Private key
         :param local_filepath: The file and the full path on your local machine
         :param remote_filepath: The path and filename on the remote location
         :param confirm: If you want to confirm the upload
```

### Comparing `salure_helpers_ftp-1.5.4/setup.py` & `salure_helpers_ftp-1.5.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='salure_helpers_ftp',
-    version='1.5.4',
+    version='1.5.5',
     description='FTP wrapper from Salure',
     long_description='FTP wrapper from Salure',
     author='D&A Salure',
     author_email='support@salureconnnect.com',
     packages=["salure_helpers.ftp"],
     license='Salure License',
     install_requires=[
```

