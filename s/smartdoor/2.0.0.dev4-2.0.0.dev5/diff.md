# Comparing `tmp/smartdoor-2.0.0.dev4.tar.gz` & `tmp/smartdoor-2.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev4.tar` & `smartdoor-2.0.0.dev5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev4/.gitignore
--rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev4/LICENSE.md
--rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev4/README.md
--rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev4/pyproject.toml
--rw-r--r--   0        0        0     9391 2023-07-25 09:57:14.979500 smartdoor-2.0.0.dev4/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev4/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev4/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     5180 2023-07-25 06:46:56.039339 smartdoor-2.0.0.dev4/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev4/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev4/smartdoor/logging.conf
--rw-r--r--   0        0        0      220 2023-07-25 09:42:58.357471 smartdoor-2.0.0.dev4/smartdoor/pigpio.service
--rw-r--r--   0        0        0     8784 2023-07-25 06:45:18.147013 smartdoor-2.0.0.dev4/smartdoor/smartdoor.py
--rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev4/smartdoor/smartdoor.service
--rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev4/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev5/.gitignore
+-rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev5/LICENSE.md
+-rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev5/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev5/pyproject.toml
+-rw-r--r--   0        0        0     9391 2023-07-25 10:28:45.411313 smartdoor-2.0.0.dev5/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev5/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev5/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     5180 2023-07-25 10:14:25.177153 smartdoor-2.0.0.dev5/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev5/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev5/smartdoor/logging.conf
+-rw-r--r--   0        0        0      222 2023-07-25 10:31:54.119674 smartdoor-2.0.0.dev5/smartdoor/pigpio.service
+-rw-r--r--   0        0        0     8856 2023-07-25 10:29:16.968711 smartdoor-2.0.0.dev5/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev5/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev5/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev4/.gitignore` & `smartdoor-2.0.0.dev5/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/LICENSE.md` & `smartdoor-2.0.0.dev5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/README.md` & `smartdoor-2.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/pyproject.toml` & `smartdoor-2.0.0.dev5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/smartdoor/__init__.py` & `smartdoor-2.0.0.dev5/smartdoor/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev4"
+__version__ = "2.0.0.dev5"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
```

### Comparing `smartdoor-2.0.0.dev4/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev5/smartdoor/core/authenticate.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev5/smartdoor/core/smartlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """
         self.logger.debug("locking sequence started")
 
         # Green LED off
         self.led_green.off()
 
         # Red LED blinking
-        self.led_red.blink(on_time=0.2, off_time=0.2)
+        self.led_red.blink(on_time=0.1, off_time=0.1)
 
         # sound buzzer
         self.buzzer.beep(on_time=0.1, off_time=0.05, n=2)
 
         # control servomotor
         self.servo.min()
         sleep(0.5)
@@ -165,15 +165,15 @@
         """
         self.logger.debug("unlocking sequence started")
 
         # Red LED off
         self.led_red.off()
 
         # Green LED blinking
-        self.led_green.blink(on_time=0.2, off_time=0.2)
+        self.led_green.blink(on_time=0.1, off_time=0.1)
 
         # sound buzzer
         self.buzzer.beep(on_time=0.1, off_time=0.05, n=3)
 
         # control servomotor
         self.servo.max()
         sleep(0.5)
```

### Comparing `smartdoor-2.0.0.dev4/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev5/smartdoor/default_config.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/smartdoor/logging.conf` & `smartdoor-2.0.0.dev5/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev4/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev5/smartdoor/smartdoor.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,14 +222,17 @@
             self.lock()
             action = "LOCK"
             self.logger.info(f"locked by {user}")
 
         # post to IFTTT
         self.post_ifttt(user=user, action=action)
 
+        # pause for 1 sec to avoid multiple execution
+        sleep(1)
+
     def warning_sequence(self) -> None:
         """Warning sequence when an unauthorized user touched the reader."""
         # Blink red LED and sound buzzer
         self.led_green.off()
         self.led_red.blink(on_time=0.1, off_time=0.1)
         self.buzzer.beep(iteration=2, dt=0.5, interval=0.1)
```

### Comparing `smartdoor-2.0.0.dev4/PKG-INFO` & `smartdoor-2.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdoor
-Version: 2.0.0.dev4
+Version: 2.0.0.dev5
 Summary: Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 Author-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Maintainer-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

