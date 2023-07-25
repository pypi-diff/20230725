# Comparing `tmp/iosslsniffer-0.0.1.tar.gz` & `tmp/iosslsniffer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iosslsniffer-0.0.1.tar", last modified: Wed Jun 21 15:29:44 2023, max compression
+gzip compressed data, was "iosslsniffer-0.0.2.tar", last modified: Tue Jul 25 08:38:53 2023, max compression
```

## Comparing `iosslsniffer-0.0.1.tar` & `iosslsniffer-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/iosslsniffer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/sniffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/ssl_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/syslog_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/iosslsniffer/tcp_simulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/iosslsniffer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-21 15:29:44.000000 iosslsniffer-0.0.1/iosslsniffer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-21 15:29:44.252084 iosslsniffer-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/tests/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-21 15:29:28.000000 iosslsniffer-0.0.1/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/iosslsniffer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/sniffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/ssl_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/syslog_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/iosslsniffer/tcp_simulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/iosslsniffer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 08:38:53.000000 iosslsniffer-0.0.2/iosslsniffer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:38:53.437587 iosslsniffer-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/tests/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-25 08:38:29.000000 iosslsniffer-0.0.2/tests/test_parser.py
```

### Comparing `iosslsniffer-0.0.1/PKG-INFO` & `iosslsniffer-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosslsniffer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sniffer for encrypted traffic
 Author-email: netanelc305 <netanelc305@protonmail.com>, doronz88 <doron88@gmail.com>
 Maintainer-email: netanelc305 <netanelc305@protonmail.com>, doronz88 <doron88@gmail.com>
 Project-URL: Homepage, https://github.com/netanelc305/ioSSLsniffer
 Project-URL: Bug Reports, https://github.com/netanelc305/ioSSLsniffer/issues
 Keywords: ios,jailbreak,ssl,sniffer,tls,cli,automation
 Classifier: Operating System :: iOS
```

### Comparing `iosslsniffer-0.0.1/README.md` & `iosslsniffer-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/iosslsniffer/__main__.py` & `iosslsniffer-0.0.2/iosslsniffer/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
 import click
 import coloredlogs
 import rpcclient.protocol
 from pymobiledevice3.cli.cli_common import Command
+from pymobiledevice3.lockdown_service_provider import LockdownServiceProvider
 from rpcclient.client_factory import create_client
 
 from iosslsniffer.sniffer import Filters, Sniffer
 
 GLOBAL_PREFERENCE = '/private/var/Managed Preferences/mobile/.GlobalPreferences.plist'
 CFNETWORK_KEY = 'AppleCFNetworkDiagnosticLogging'
 
@@ -25,19 +26,19 @@
 @click.group()
 def cli():
     pass
 
 
 @cli.command('setup', cls=Command)
 @click.option('-p', '--port', type=click.INT, default=rpcclient.protocol.DEFAULT_PORT, help='rpc server ip and port')
-def cli_setup(lockdown, port):
+def cli_setup(service_provider: LockdownServiceProvider, port):
     """ Setup all prerequisites required inorder to sniff the SSL traffic """
 
     def usbmux_connect():
-        return lockdown.service.mux_device.connect(port)
+        return service_provider.service.mux_device.connect(port)
 
     rpc = create_client(usbmux_connect)
 
     with rpc.preferences.sc.open(GLOBAL_PREFERENCE) as global_preferences:
         if not global_preferences.get(CFNETWORK_KEY):
             global_preferences.set(CFNETWORK_KEY, 3)
             logger.info(f'{CFNETWORK_KEY} is now set, a restart is required')
@@ -50,16 +51,16 @@
 @click.option('out_file', '-o', '--out', default='traffic.pcapng', type=click.Path(),
               help='outfile name with .pcapng extension')
 @click.option('pids', '-p', '--pid', type=click.INT, multiple=True, callback=default_none, help='filter pid list')
 @click.option('process_names', '-pn', '--process-name', callback=default_none, multiple=True,
               help='filter process name list')
 @click.option('images', '-i', '--image', multiple=True, callback=default_none, help='filter image list')
 @click.option('--black-list/--white-list', default=True, is_flag=True)
-def cli_sniff(lockdown, pids, process_names, images, out_file, black_list):
+def cli_sniff(service_provider: LockdownServiceProvider, pids, process_names, images, out_file, black_list):
     """ Sniff the traffic """
 
     filters = Filters(pids, process_names, images, black_list)
-    Sniffer(lockdown, out_file, filters=filters).sniff()
+    Sniffer(service_provider, out_file, filters=filters).sniff()
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `iosslsniffer-0.0.1/iosslsniffer/sniffer.py` & `iosslsniffer-0.0.2/iosslsniffer/sniffer.py`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/iosslsniffer/ssl_session.py` & `iosslsniffer-0.0.2/iosslsniffer/ssl_session.py`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/iosslsniffer/syslog_parser.py` & `iosslsniffer-0.0.2/iosslsniffer/syslog_parser.py`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/iosslsniffer/tcp_simulation.py` & `iosslsniffer-0.0.2/iosslsniffer/tcp_simulation.py`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/iosslsniffer.egg-info/PKG-INFO` & `iosslsniffer-0.0.2/iosslsniffer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosslsniffer
-Version: 0.0.1
+Version: 0.0.2
 Summary: Sniffer for encrypted traffic
 Author-email: netanelc305 <netanelc305@protonmail.com>, doronz88 <doron88@gmail.com>
 Maintainer-email: netanelc305 <netanelc305@protonmail.com>, doronz88 <doron88@gmail.com>
 Project-URL: Homepage, https://github.com/netanelc305/ioSSLsniffer
 Project-URL: Bug Reports, https://github.com/netanelc305/ioSSLsniffer/issues
 Keywords: ios,jailbreak,ssl,sniffer,tls,cli,automation
 Classifier: Operating System :: iOS
```

### Comparing `iosslsniffer-0.0.1/pyproject.toml` & `iosslsniffer-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "iosslsniffer"
-version = "0.0.1"
+version = "0.0.2"
 description = "Sniffer for encrypted traffic"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
 keywords = ["ios", "jailbreak", "ssl", "sniffer", "tls", "cli", "automation"]
 authors = [
     { name = "netanelc305", email = "netanelc305@protonmail.com" },
```

### Comparing `iosslsniffer-0.0.1/tests/test_filters.py` & `iosslsniffer-0.0.2/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `iosslsniffer-0.0.1/tests/test_parser.py` & `iosslsniffer-0.0.2/tests/test_parser.py`

 * *Files identical despite different names*

