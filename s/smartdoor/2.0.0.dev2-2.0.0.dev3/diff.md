# Comparing `tmp/smartdoor-2.0.0.dev2.tar.gz` & `tmp/smartdoor-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev2.tar` & `smartdoor-2.0.0.dev3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev2/.gitignore
--rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev2/LICENSE.md
--rw-r--r--   0        0        0     2378 2023-07-24 08:20:10.549946 smartdoor-2.0.0.dev2/README.md
--rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev2/pyproject.toml
--rw-r--r--   0        0        0     7937 2023-07-24 06:15:07.509887 smartdoor-2.0.0.dev2/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev2/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev2/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     4968 2023-05-20 08:34:48.408198 smartdoor-2.0.0.dev2/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev2/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev2/smartdoor/logging.conf
--rw-r--r--   0        0        0     8775 2023-07-22 08:42:24.603572 smartdoor-2.0.0.dev2/smartdoor/smartdoor.py
--rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev2/smartdoor/smartdoor.service
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev2/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev3/.gitignore
+-rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev3/LICENSE.md
+-rw-r--r--   0        0        0     3481 2023-07-25 09:48:35.392457 smartdoor-2.0.0.dev3/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev3/pyproject.toml
+-rw-r--r--   0        0        0     9395 2023-07-25 09:33:31.408248 smartdoor-2.0.0.dev3/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev3/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev3/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     5180 2023-07-25 06:46:56.039339 smartdoor-2.0.0.dev3/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev3/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev3/smartdoor/logging.conf
+-rw-r--r--   0        0        0      220 2023-07-25 09:42:58.357471 smartdoor-2.0.0.dev3/smartdoor/pigpio.service
+-rw-r--r--   0        0        0     8784 2023-07-25 06:45:18.147013 smartdoor-2.0.0.dev3/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev3/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     4802 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev3/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev2/.gitignore` & `smartdoor-2.0.0.dev3/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/LICENSE.md` & `smartdoor-2.0.0.dev3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/README.md` & `smartdoor-2.0.0.dev3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,27 +4,48 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartdoor?logo=Python)
 
 [![GitHub](https://img.shields.io/github/license/munechika-koyo/cherab_phix)](https://opensource.org/licenses/BSD-3-Clause)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc. with Raspberry Pi.
 
+## Default circuit diagram
+The default circuit diagram is shown below. If you want to use other GPIO pin numbers, please edit the configuration file (see below).
+
+![circuit](docs/circuit.png) not yet updated
+
+
 ## Quick Installation
 ```bash
-python -m pip install smartdoor
+sudo python -m pip install smartdoor
 ```
 
 ## Before getting started
 
 ### `smartdoor_host` system
 Smartdoor Host system which serves the web application for NFC key management must be run. Please
 install and deploy it in adavnce. ([see here](https://github.com/munechika-koyo/smartdoor_host)).
 
 ### pigpio library
-`pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance. ([see here](http://abyz.me.uk/rpi/pigpio/download.html))
+`pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance ([see here](http://abyz.me.uk/rpi/pigpio/download.html)) and run the daemon by the following command:
+```bash
+sudo pigpiod
+```
+It is recommended to run the daemon automatically at the system startup. If `pigpio` is installed
+and impotable from Python, `smartdoor` package will automatically register it in `systemd` service (see below).
+
+### NFC reader permission
+To access NFC reader, the permission of the device file must be set. Please execute the following.
+```bash
+sudo sh -c 'echo SUBSYSTEM==\"usb\", ACTION==\"add\", ATTRS{idVendor}==\"054c\", ATTRS{idProduct}==\"06c3\", GROUP=\"plugdev\" >> /etc/udev/rules.d/nfcdev.rules'
+sudo udevadm control -R
+```
+Then, reboot the system.
+This instruction is based on the result of `python -m nfc` command. If you use other NFC reader, please change the `idVendor` and `idProduct` according to your device.
+
 
 ## How to use
 
 Almost all the operations are done by the `smartdoor` command. Please see the help message for the
 details:
 ```bash
 smartdoor --help
@@ -49,15 +70,18 @@
 
 ### 3. Set up the auto start
 The main program can be automatically run by `systemd` service. To register the `smartdoor.service`
 to `systemd`, execute the following command:
 ```bash
 smartdoor service --register
 ```
-Then, the service will be ready for start. To manually start it, execute the following command:
+Then, the service will be ready for start. Simaltenously, the `pigpiod` service will be registered
+if `pigpio` library is installed.
+
+To manually start it, execute the following command:
 ```bash
 smartdoor service --start
 ```
 
 Please see the help message for other options:
 ```bash
 smartdoor service --help
```

### Comparing `smartdoor-2.0.0.dev2/pyproject.toml` & `smartdoor-2.0.0.dev3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/smartdoor/__init__.py` & `smartdoor-2.0.0.dev3/smartdoor/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 This system is designed to be used with Raspberry Pi.
 
 Some CLIs including main sequence is implemented here.
 """
 from __future__ import annotations
 
 import subprocess
+from importlib.util import find_spec
 from logging import config as log_config
 from logging import getLogger
 from pathlib import Path
 from pprint import pformat
 
 import rich_click as click
 
@@ -21,15 +22,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev2"
+__version__ = "2.0.0.dev3"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
@@ -60,15 +61,15 @@
     try:
         while True:
             tag = door.wait_for_touched()
 
             # If buttom is pushed
             if tag is None:
                 door.led_button.blink(on_time=0.2, off_time=0.2)
-                door.door_sequence(user="Button pusher")
+                door.door_sequence(user="Button operator")
                 door.led_button.on()
                 continue
 
             # If NFC card is detected
             elif bool(tag):
                 user = door.authenticate(tag)
 
@@ -91,15 +92,15 @@
 
     finally:
         door.close()
 
 
 @cli.command()
 @click.option("--debug", "-d", is_flag=True, help="show debug log")
-def show_log(debug: bool):
+def logs(debug: bool):
     """Show logs of SmartDoor system.
 
     logs are stored in `~/smartdoor.log` or `~/smartdoor_debug.log`. If you want to show debug log,
     use `--debug` option.
     """
     log = Path().home() / "smartdoor.log" if not debug else Path().home() / "smartdoor_debug.log"
 
@@ -157,34 +158,63 @@
 
     If you want to register/unregister smartdoor system to/from systemd, use `--register` or
     `--unregister` option. If choosing `--register` option, smartdoor system will be ready for start
     automatically.
 
     You can also start/stop/restart service by `--start`, `--stop`, `--restart` option. If you want
     to show service status, use `--status` option.
+
+    If `pigpio` is installed, launching `pigpio` daemon is also registered to systemd automatically.
     """
     if register:
+        # Register pigpio daemon to systemd
+        if find_spec("pigpio") is not None:
+            try:
+                service_file = Path(__file__).parent / "pigpiod.service"
+                subprocess.run(
+                    ["sudo", "systemctl", "link", str(service_file)],
+                    check=True,
+                )
+                subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
+                subprocess.run(["sudo", "systemctl", "enable", "pigpiod.service"], check=True)
+                click.echo("registered pigpio daemon to systemd")
+            except subprocess.CalledProcessError as e:
+                click.echo(e)
+                click.echo("failed to register pigpio daemon to systemd")
+
+        # Register smartdoor service to systemd
         try:
             service_file = Path(__file__).parent / "smartdoor.service"
             subprocess.run(
-                ["sudo", "ln", "-s", str(service_file), "/etc/systemd/system/smartdoor.service"],
+                ["sudo", "systemctl", "link", str(service_file)],
                 check=True,
             )
             subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
             subprocess.run(["sudo", "systemctl", "enable", "smartdoor.service"], check=True)
             click.echo("registered service to systemd")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to register service to systemd")
 
     elif unregister:
+        # Unregister pigpio daemon from systemd
+        if find_spec("pigpio") is not None:
+            try:
+                subprocess.run(["sudo", "systemctl", "stop", "pigpiod.service"], check=True)
+                subprocess.run(["sudo", "systemctl", "disable", "pigpiod.service"], check=True)
+                subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
+                click.echo("unregistered pigpio daemon from systemd")
+            except subprocess.CalledProcessError as e:
+                click.echo(e)
+                click.echo("failed to unregister pigpio daemon from systemd")
+
+        # Unregister smartdoor service from systemd
         try:
             subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
             subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"], check=True)
-            subprocess.run(["sudo", "rm", "/etc/systemd/system/smartdoor.service"], check=True)
             subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
             click.echo("unregistered service from systemd")
         except subprocess.CalledProcessError as e:
             click.echo(e)
             click.echo("failed to unregister service from systemd")
 
     elif start:
```

### Comparing `smartdoor-2.0.0.dev2/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev3/smartdoor/core/authenticate.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev3/smartdoor/core/smartlock.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,25 +43,26 @@
         # set pin factory
         try:
             from gpiozero.pins.pigpio import PiGPIOFactory
 
             Device.pin_factory = PiGPIOFactory()
             self.logger.debug("using pigpio pin factory")
 
-        except ModuleNotFoundError:
+        except Exception:
             self.logger.debug("using defalut pin factory")
 
         # validate pin assignment
         self.pins = pins
 
         # Initialize GPIO devices
         # === LED ===
         self.led_red = LED(pins["LED_red"])
         self.led_green = LED(pins["LED_green"])
         self.led_button = LED(pins["LED_button"])
+        self.led_button.on()
 
         # === Push button switch ===
         self.button = Button(pins["button"])
 
         # === Buzzer ===
         self.buzzer = Buzzer(pins["buzzer"])
 
@@ -104,14 +105,21 @@
         return self._locked
 
     @locked.setter
     def locked(self, value):
         if not isinstance(value, bool):
             raise TypeError("locked must be a bool value")
         self._locked = value
+        # update LED status
+        if self._locked:
+            self.led_red.on()
+            self.led_green.off()
+        else:
+            self.led_red.off()
+            self.led_green.on()
 
     def lock(self) -> None:
         """Excute Locking sequence.
 
         The detail of the sequence is as follows:
 
         1. Green LED off
```

### Comparing `smartdoor-2.0.0.dev2/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev3/smartdoor/default_config.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/smartdoor/logging.conf` & `smartdoor-2.0.0.dev3/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev2/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev3/smartdoor/smartdoor.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         """
         rdwr_options = {
             "targets": ["212F"],  # detect only Felica
             "on-connect": lambda tag: False,
             "iterations": 5,
             "interval": 0.5,
         }
-        tag = self.clf.connect(rdwr=rdwr_options, terminate=self.button.is_pushed)
+        tag = self.clf.connect(rdwr=rdwr_options, terminate=lambda: self.button.is_pressed)
 
         return tag
 
     def authenticate(self, tag: Tag) -> str | None:
         """Authenticate the approved user.
 
         This method authenticates the user by the IDm of the NFC card.
```

### Comparing `smartdoor-2.0.0.dev2/PKG-INFO` & `smartdoor-2.0.0.dev3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdoor
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 Author-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Maintainer-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -37,27 +37,48 @@
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/smartdoor?logo=Python)
 
 [![GitHub](https://img.shields.io/github/license/munechika-koyo/cherab_phix)](https://opensource.org/licenses/BSD-3-Clause)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc. with Raspberry Pi.
 
+## Default circuit diagram
+The default circuit diagram is shown below. If you want to use other GPIO pin numbers, please edit the configuration file (see below).
+
+![circuit](docs/circuit.png) not yet updated
+
+
 ## Quick Installation
 ```bash
-python -m pip install smartdoor
+sudo python -m pip install smartdoor
 ```
 
 ## Before getting started
 
 ### `smartdoor_host` system
 Smartdoor Host system which serves the web application for NFC key management must be run. Please
 install and deploy it in adavnce. ([see here](https://github.com/munechika-koyo/smartdoor_host)).
 
 ### pigpio library
-`pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance. ([see here](http://abyz.me.uk/rpi/pigpio/download.html))
+`pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance ([see here](http://abyz.me.uk/rpi/pigpio/download.html)) and run the daemon by the following command:
+```bash
+sudo pigpiod
+```
+It is recommended to run the daemon automatically at the system startup. If `pigpio` is installed
+and impotable from Python, `smartdoor` package will automatically register it in `systemd` service (see below).
+
+### NFC reader permission
+To access NFC reader, the permission of the device file must be set. Please execute the following.
+```bash
+sudo sh -c 'echo SUBSYSTEM==\"usb\", ACTION==\"add\", ATTRS{idVendor}==\"054c\", ATTRS{idProduct}==\"06c3\", GROUP=\"plugdev\" >> /etc/udev/rules.d/nfcdev.rules'
+sudo udevadm control -R
+```
+Then, reboot the system.
+This instruction is based on the result of `python -m nfc` command. If you use other NFC reader, please change the `idVendor` and `idProduct` according to your device.
+
 
 ## How to use
 
 Almost all the operations are done by the `smartdoor` command. Please see the help message for the
 details:
 ```bash
 smartdoor --help
@@ -82,15 +103,18 @@
 
 ### 3. Set up the auto start
 The main program can be automatically run by `systemd` service. To register the `smartdoor.service`
 to `systemd`, execute the following command:
 ```bash
 smartdoor service --register
 ```
-Then, the service will be ready for start. To manually start it, execute the following command:
+Then, the service will be ready for start. Simaltenously, the `pigpiod` service will be registered
+if `pigpio` library is installed.
+
+To manually start it, execute the following command:
 ```bash
 smartdoor service --start
 ```
 
 Please see the help message for other options:
 ```bash
 smartdoor service --help
```

