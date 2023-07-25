# Comparing `tmp/salure_helpers_ftp-1.5.2.tar.gz` & `tmp/salure_helpers_ftp-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/salure_helpers_ftp-1.5.2.tar", last modified: Mon Jul 24 14:07:04 2023, max compression
+gzip compressed data, was "dist/salure_helpers_ftp-1.5.4.tar", last modified: Tue Jul 25 09:57:11 2023, max compression
```

## Comparing `salure_helpers_ftp-1.5.2.tar` & `salure_helpers_ftp-1.5.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/
--rw-r--r--   0 root         (0) root         (0)      253 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/ftps.py
--rw-rw-rw-   0 root         (0) root         (0)     6259 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/salure_helpers/ftp/sftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      253 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      343 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       79 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/salure_helpers_ftp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-24 14:07:04.000000 salure_helpers_ftp-1.5.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      493 2023-07-24 14:06:55.000000 salure_helpers_ftp-1.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)       81 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10718 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/ftps.py
+-rw-rw-rw-   0 root         (0) root         (0)     6344 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/salure_helpers/ftp/sftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      343 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/salure_helpers_ftp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 09:57:11.000000 salure_helpers_ftp-1.5.4/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      518 2023-07-25 09:56:58.000000 salure_helpers_ftp-1.5.4/setup.py
```

### Comparing `salure_helpers_ftp-1.5.2/salure_helpers/ftp/ftps.py` & `salure_helpers_ftp-1.5.4/salure_helpers/ftp/ftps.py`

 * *Files identical despite different names*

### Comparing `salure_helpers_ftp-1.5.2/salure_helpers/ftp/sftp.py` & `salure_helpers_ftp-1.5.4/salure_helpers/ftp/sftp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from paramiko.client import SSHClient, AutoAddPolicy
 from paramiko.pkey import PKey
 from paramiko import RSAKey
 from paramiko.sftp_attr import SFTPAttributes
+import pysftp
 from typing import Union, List
 from salure_helpers.salureconnect import SalureConnect
 from stat import S_ISREG
 
 
 class SFTP(SalureConnect):
     def __init__(self, label: Union[str, List], debug=False):
@@ -20,19 +21,20 @@
         self.debug = debug
         if self.debug:
             print(credentials)
         self.host = credentials['host']
         self.port = 22 if credentials['port'] is None else credentials['port']
         self.username = credentials['username']
         self.password = credentials['password']
-        # untested
-        self.private_key = RSAKey.from_private_key(open(credentials['private_key_path'], mode='r'), password=credentials['private_key_password']) if credentials['private_key_path'] is not None else None
-        policy = AutoAddPolicy()
-        self.client = SSHClient()
-        self.client.set_missing_host_key_policy(policy)
+        self.cnopts = pysftp.CnOpts()
+        self.cnopts.hostkeys = None
+        self.private_key_path = None
+        if credentials['private_key_path'] is not None:
+            self.private_key_path = credentials['private_key_path']
+            self.private_key_password = credentials['private_key_password']
 
     def upload_file(self, local_filepath, remote_filepath, confirm=True) -> SFTPAttributes:
         """
         Upload a single file to a remote location. If there is no Private key
         :param local_filepath: The file and the full path on your local machine
         :param remote_filepath: The path and filename on the remote location
         :param confirm: If you want to confirm the upload
@@ -74,21 +76,22 @@
         """
         Download a single file
         :param remote_path: the path where the remote file exists
         :param remote_file: the remote file itself
         :param local_path: the path where the file needs to be downloaded to
         :return: a file object
         """
-        if self.private_key is None:
-            self.client.connect(hostname=self.host, port=self.port, username=self.username, password=self.password)
+        if self.private_key_path == None:
+            connection = pysftp.Connection(host=self.host, port=self.port, username=self.username, password=self.password, cnopts=self.cnopts)
         else:
-            self.client.connect(hostname=self.host, port=self.port, username=self.username, pkey=self.private_key)
-        sftp = self.client.open_sftp()
-        sftp.get(remotepath=f'{remote_path}{remote_file}', localpath=f'{local_path}/{remote_file}')
-        self.client.close()
+            connection = pysftp.Connection(host=self.host, port=self.port, username=self.username, private_key=self.private_key_path, private_key_pass=self.private_key_pass, cnopts=self.cnopts)
+
+        file = connection.get(remotepath=f'{remote_path}{remote_file}', localpath=f'{local_path}/{remote_file}')
+        connection.close()
+        return file
 
     def make_dir(self, remote_path, new_dir_name):
         """
         Create a new folder on a remote location
         :param remote_path: The location where you want to create the new folder
         :param new_dir_name: The name of the new folder
         :return: a status if creating succeeded or not
```

