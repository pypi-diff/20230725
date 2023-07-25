# Comparing `tmp/commonutil-net-fileservice-0.0.2.tar.gz` & `tmp/commonutil-net-fileservice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonutil-net-fileservice-0.0.2.tar", last modified: Thu Jun 29 19:22:43 2023, max compression
+gzip compressed data, was "commonutil-net-fileservice-0.1.2.tar", last modified: Tue Jul 25 18:48:14 2023, max compression
```

## Comparing `commonutil-net-fileservice-0.0.2.tar` & `commonutil-net-fileservice-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 vincentl  (1000) vincentl  (1000)        0 2023-06-29 19:22:43.164771 commonutil-net-fileservice-0.0.2/
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)      467 2023-06-29 19:22:43.164771 commonutil-net-fileservice-0.0.2/PKG-INFO
-drwxrwxr-x   0 vincentl  (1000) vincentl  (1000)        0 2023-06-29 19:22:43.164771 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)        0 2023-06-23 15:41:28.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/__init__.py
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)     2532 2023-06-25 14:59:45.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/config.py
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)    14575 2023-06-25 15:46:39.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/paramikosftp.py
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)     4312 2023-06-25 16:00:07.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/paramikosubexec.py
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)    11779 2023-06-25 15:19:12.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/pyftpdlib.py
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)     7507 2023-06-25 15:59:40.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/scp.py
-drwxrwxr-x   0 vincentl  (1000) vincentl  (1000)        0 2023-06-29 19:22:43.164771 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice.egg-info/
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)      467 2023-06-29 19:22:43.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice.egg-info/PKG-INFO
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)      447 2023-06-29 19:22:43.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice.egg-info/SOURCES.txt
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)        1 2023-06-29 19:22:43.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice.egg-info/dependency_links.txt
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)       27 2023-06-29 19:22:43.000000 commonutil-net-fileservice-0.0.2/commonutil_net_fileservice.egg-info/top_level.txt
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)       38 2023-06-29 19:22:43.164771 commonutil-net-fileservice-0.0.2/setup.cfg
--rw-rw-r--   0 vincentl  (1000) vincentl  (1000)      617 2023-06-24 22:08:30.000000 commonutil-net-fileservice-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:48:14.751082 commonutil-net-fileservice-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-25 18:48:14.751082 commonutil-net-fileservice-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:48:14.747082 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/paramikosftp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/paramikosubexec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/pyftpdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:48:14.751082 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-25 18:48:14.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-25 18:48:14.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:48:14.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 18:48:14.000000 commonutil-net-fileservice-0.1.2/commonutil_net_fileservice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:48:14.751082 commonutil-net-fileservice-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-25 18:48:00.000000 commonutil-net-fileservice-0.1.2/setup.py
```

### Comparing `commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/config.py` & `commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from typing import Any, Callable, Iterable, Mapping, Optional
 import logging
 import os
 
 _log = logging.getLogger(__name__)
 
-_REV = "0.0.2; 54e6001c024d5e934f47fe6f4451084986e8f9f0"  # REV-CONSTANT:full 5d022db7d38f580a850cd995e26a6c2f
+_REV = "0.1.2; fdb796342e2f009a73ce4638d37e2a3383af8919"  # REV-CONSTANT:full 5d022db7d38f580a850cd995e26a6c2f
 
 DEFAULT_REV_FILENAME = "_rev-info.txt"
 DEFAULT_REV_CONTENT = _REV + "\n"
 
 
 def _default_credential_checker(u: User, remote_credential: str) -> bool:
 	return (u.credential == remote_credential)
```

### Comparing `commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/paramikosftp.py` & `commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/paramikosftp.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import shutil
 import socketserver
 import time
 
 import paramiko
 
 from commonutil_net_fileservice.config import (DEFAULT_REV_CONTENT, DEFAULT_REV_FILENAME, User, make_users_map)
-from commonutil_net_fileservice.paramikosubexec import (run_rsync_exec, run_scp_sink)
+from commonutil_net_fileservice.paramikosubexec import (run_rsync_exec, RsyncOptions, run_scp_sink)
 
 _log = logging.getLogger(__name__)
 
 
 def open_mode_from_flags(flags) -> str:
 	if flags & os.O_EXCL:
 		return 'xb'
@@ -45,15 +45,16 @@
 
 
 def make_sftp_attr(file_name: str, file_content: bytes) -> paramiko.SFTPAttributes:
 	fattr = paramiko.SFTPAttributes()
 	fattr.st_size = len(file_content)
 	fattr.st_uid = 0
 	fattr.st_gid = 0
-	fattr.st_mode = 0o0444
+	fattr.st_mode = 0o100444
+	fattr.st_mtime = int(time.time())
 	fattr.filename = file_name
 	return fattr
 
 
 class SFTPHandle(paramiko.SFTPHandle):
 	# pylint: disable=too-many-arguments
 	def __init__(self, fp, flags, local_path, rel_path, report_callable, stat_object=None):
@@ -274,34 +275,34 @@
 	__slots__ = (
 			'base_folder_path',
 			'users',
 			'process_callable',
 			'v_rev_filename',
 			'v_rev_content',
 			'v_rev_stat',
-			'binpath_rsync',
+			'rsync_opts',
 			'_users_lck',
 	)
 
 	# pylint: disable=too-many-arguments
 	def __init__(self,
 					base_folder_path: str,
 					users: Iterable[User],
 					process_callable: Callable[[str, str, str, str], None],
 					v_rev_filename: str = DEFAULT_REV_FILENAME,
 					v_rev_content: str = DEFAULT_REV_CONTENT,
-					binpath_rsync: Optional[str] = None) -> None:
+					rsync_opts: Optional[RsyncOptions] = None) -> None:
 		super().__init__()
 		self.base_folder_path = base_folder_path
 		self.users = make_users_map(users)
 		self.process_callable = process_callable
 		self.v_rev_filename = v_rev_filename
 		self.v_rev_content = (v_rev_content.strip() + "\n").encode('utf-8', 'ignore')
 		self.v_rev_stat = make_sftp_attr(v_rev_filename, self.v_rev_content)
-		self.binpath_rsync = binpath_rsync
+		self.rsync_opts = rsync_opts
 		self._users_lck = _thread.allocate_lock()
 
 	def update_users(self, users: Iterable[User]):
 		rec = make_users_map(users)
 		with self._users_lck:
 			to_drop = []
 			for k in self.users:
@@ -335,16 +336,16 @@
 		if len(cmdpart) < 2:
 			raise Exception('low argument count', cmdpart)
 		cmdtarget = cmdpart[0]
 		_log.info("run: [%s] as [%r]", cmdtarget, remote_username)
 		user_folder_path = os.path.abspath(os.path.join(self.base_folder_path, u.username))
 		report_callable = _ReportCallableWrap(channel, u, self.process_callable)
 		if cmdtarget in ('rsync', '/bin/rsync', '/usr/bin/rsync'):
-			if self.binpath_rsync:
-				_thread.start_new_thread(run_rsync_exec, (user_folder_path, report_callable, channel, cmdpart))
+			if self.rsync_opts:
+				_thread.start_new_thread(run_rsync_exec, (remote_username, user_folder_path, report_callable, channel, cmdpart, self.rsync_opts))
 			else:
 				_log.warning("requested rsync but rsync executable path is not configurated")
 				return False
 		elif cmdtarget in ('scp', '/bin/scp', '/usr/bin/scp'):
 			_thread.start_new_thread(run_scp_sink, (user_folder_path, report_callable, channel, cmdpart))
 		else:
 			raise Exception('unknown command', cmdtarget, command)
@@ -418,18 +419,18 @@
 					key_file_path: str,
 					key_bits: int,
 					base_folder_path: str,
 					users: Iterable[User],
 					process_callable: Callable[[str, str, str, str], None],
 					v_rev_filename: str = DEFAULT_REV_FILENAME,
 					v_rev_content: str = DEFAULT_REV_CONTENT,
-					binpath_rsync: Optional[str] = None) -> None:
+					rsync_opts: Optional[RsyncOptions] = None) -> None:
 		super().__init__((server_host, server_port), SSHLinkHandler)
 		try:
 			self.host_pkey = paramiko.RSAKey.from_private_key_file(key_file_path)
 		except FileNotFoundError:
 			self.host_pkey = paramiko.RSAKey.generate(key_bits)
 			self.host_pkey.write_private_key_file(key_file_path)
-		self.server_impl = ServerImpl(base_folder_path, users, process_callable, v_rev_filename, v_rev_content, binpath_rsync)
+		self.server_impl = ServerImpl(base_folder_path, users, process_callable, v_rev_filename, v_rev_content, rsync_opts)
 
 	def update_users(self, users: Iterable[User]):
 		self.server_impl.update_users(users)
```

### Comparing `commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/pyftpdlib.py` & `commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/pyftpdlib.py`

 * *Files identical despite different names*

### Comparing `commonutil-net-fileservice-0.0.2/commonutil_net_fileservice/scp.py` & `commonutil-net-fileservice-0.1.2/commonutil_net_fileservice/scp.py`

 * *Files identical despite different names*

