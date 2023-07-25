# Comparing `tmp/smartdoor-2.0.0.dev3.tar.gz` & `tmp/smartdoor-2.0.0.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev3.tar` & `smartdoor-2.0.0.dev4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev3/.gitignore
--rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev3/LICENSE.md
--rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev3/README.md
--rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev3/pyproject.toml
--rw-r--r--   0        0        0     9395 2023-07-25 09:33:31.408248 smartdoor-2.0.0.dev3/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev3/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev3/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     5180 2023-07-25 06:46:56.039339 smartdoor-2.0.0.dev3/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev3/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev3/smartdoor/logging.conf
--rw-r--r--   0        0        0      220 2023-07-25 09:42:58.357471 smartdoor-2.0.0.dev3/smartdoor/pigpio.service
--rw-r--r--   0        0        0     8784 2023-07-25 06:45:18.147013 smartdoor-2.0.0.dev3/smartdoor/smartdoor.py
--rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev3/smartdoor/smartdoor.service
--rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev3/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev4/.gitignore
+-rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev4/LICENSE.md
+-rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev4/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev4/pyproject.toml
+-rw-r--r--   0        0        0     9391 2023-07-25 09:57:14.979500 smartdoor-2.0.0.dev4/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev4/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev4/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     5180 2023-07-25 06:46:56.039339 smartdoor-2.0.0.dev4/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev4/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev4/smartdoor/logging.conf
+-rw-r--r--   0        0        0      220 2023-07-25 09:42:58.357471 smartdoor-2.0.0.dev4/smartdoor/pigpio.service
+-rw-r--r--   0        0        0     8784 2023-07-25 06:45:18.147013 smartdoor-2.0.0.dev4/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev4/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev4/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev3/.gitignore` & `smartdoor-2.0.0.dev4/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/LICENSE.md` & `smartdoor-2.0.0.dev4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/README.md` & `smartdoor-2.0.0.dev4/README.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/pyproject.toml` & `smartdoor-2.0.0.dev4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/smartdoor/__init__.py` & `smartdoor-2.0.0.dev4/smartdoor/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev3"
+__version__ = "2.0.0.dev4"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
@@ -165,21 +165,21 @@
 
     If `pigpio` is installed, launching `pigpio` daemon is also registered to systemd automatically.
     """
     if register:
         # Register pigpio daemon to systemd
         if find_spec("pigpio") is not None:
             try:
-                service_file = Path(__file__).parent / "pigpiod.service"
+                service_file = Path(__file__).parent / "pigpio.service"
                 subprocess.run(
                     ["sudo", "systemctl", "link", str(service_file)],
                     check=True,
                 )
                 subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
-                subprocess.run(["sudo", "systemctl", "enable", "pigpiod.service"], check=True)
+                subprocess.run(["sudo", "systemctl", "enable", "pigpio.service"], check=True)
                 click.echo("registered pigpio daemon to systemd")
             except subprocess.CalledProcessError as e:
                 click.echo(e)
                 click.echo("failed to register pigpio daemon to systemd")
 
         # Register smartdoor service to systemd
         try:
@@ -195,16 +195,16 @@
             click.echo(e)
             click.echo("failed to register service to systemd")
 
     elif unregister:
         # Unregister pigpio daemon from systemd
         if find_spec("pigpio") is not None:
             try:
-                subprocess.run(["sudo", "systemctl", "stop", "pigpiod.service"], check=True)
-                subprocess.run(["sudo", "systemctl", "disable", "pigpiod.service"], check=True)
+                subprocess.run(["sudo", "systemctl", "stop", "pigpio.service"], check=True)
+                subprocess.run(["sudo", "systemctl", "disable", "pigpio.service"], check=True)
                 subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
                 click.echo("unregistered pigpio daemon from systemd")
             except subprocess.CalledProcessError as e:
                 click.echo(e)
                 click.echo("failed to unregister pigpio daemon from systemd")
 
         # Unregister smartdoor service from systemd
```

### Comparing `smartdoor-2.0.0.dev3/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev4/smartdoor/core/authenticate.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev4/smartdoor/core/smartlock.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev4/smartdoor/default_config.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/smartdoor/logging.conf` & `smartdoor-2.0.0.dev4/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev4/smartdoor/smartdoor.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev3/PKG-INFO` & `smartdoor-2.0.0.dev4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdoor
-Version: 2.0.0.dev3
+Version: 2.0.0.dev4
 Summary: Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 Author-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Maintainer-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

