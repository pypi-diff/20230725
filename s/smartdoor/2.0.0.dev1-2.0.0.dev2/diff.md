# Comparing `tmp/smartdoor-2.0.0.dev1.tar.gz` & `tmp/smartdoor-2.0.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartdoor-2.0.0.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "smartdoor-2.0.0.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `smartdoor-2.0.0.dev1.tar` & `smartdoor-2.0.0.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev1/.gitignore
--rw-r--r--   0        0        0     1136 2023-05-18 06:25:36.917565 smartdoor-2.0.0.dev1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev1/LICENSE.md
--rw-r--r--   0        0        0     2025 2023-07-22 10:51:48.525680 smartdoor-2.0.0.dev1/README.md
--rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev1/pyproject.toml
--rw-r--r--   0        0        0     6155 2023-07-22 10:50:18.729682 smartdoor-2.0.0.dev1/smartdoor/__init__.py
--rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev1/smartdoor/core/__init__.py
--rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev1/smartdoor/core/authenticate.py
--rw-r--r--   0        0        0     4968 2023-05-20 08:34:48.408198 smartdoor-2.0.0.dev1/smartdoor/core/smartlock.py
--rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev1/smartdoor/default_config.toml
--rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev1/smartdoor/logging.conf
--rw-r--r--   0        0        0     8775 2023-07-22 08:42:24.603572 smartdoor-2.0.0.dev1/smartdoor/smartdoor.py
--rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev1/smartdoor/smartdoor.service
--rw-r--r--   0        0        0     3346 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1839 2023-05-19 06:36:25.675356 smartdoor-2.0.0.dev2/.gitignore
+-rw-r--r--   0        0        0     1134 2023-07-25 04:27:54.682023 smartdoor-2.0.0.dev2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1512 2023-05-17 14:36:57.361107 smartdoor-2.0.0.dev2/LICENSE.md
+-rw-r--r--   0        0        0     2378 2023-07-24 08:20:10.549946 smartdoor-2.0.0.dev2/README.md
+-rw-r--r--   0        0        0     1861 2023-07-22 10:50:43.482784 smartdoor-2.0.0.dev2/pyproject.toml
+-rw-r--r--   0        0        0     7937 2023-07-24 06:15:07.509887 smartdoor-2.0.0.dev2/smartdoor/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-17 14:44:02.403787 smartdoor-2.0.0.dev2/smartdoor/core/__init__.py
+-rw-r--r--   0        0        0     3244 2023-05-20 08:34:52.724385 smartdoor-2.0.0.dev2/smartdoor/core/authenticate.py
+-rw-r--r--   0        0        0     4968 2023-05-20 08:34:48.408198 smartdoor-2.0.0.dev2/smartdoor/core/smartlock.py
+-rw-r--r--   0        0        0     2065 2023-07-22 10:47:46.218895 smartdoor-2.0.0.dev2/smartdoor/default_config.toml
+-rw-r--r--   0        0        0      794 2023-05-19 06:31:54.619552 smartdoor-2.0.0.dev2/smartdoor/logging.conf
+-rw-r--r--   0        0        0     8775 2023-07-22 08:42:24.603572 smartdoor-2.0.0.dev2/smartdoor/smartdoor.py
+-rw-r--r--   0        0        0      222 2023-07-21 04:14:11.966183 smartdoor-2.0.0.dev2/smartdoor/smartdoor.service
+-rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 smartdoor-2.0.0.dev2/PKG-INFO
```

### Comparing `smartdoor-2.0.0.dev1/.gitignore` & `smartdoor-2.0.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/.pre-commit-config.yaml` & `smartdoor-2.0.0.dev2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ci:
-  autofix_prs: false
+  autofix_prs: true
   autoupdate_schedule: quarterly
 
 default_language_version:
   node: 16.15.0
 
 repos:
 
@@ -20,35 +20,35 @@
   - id: check-case-conflict
   - id: check-json
   - id: check-toml
   - id: check-yaml
 
 # validate pyproject.toml
 - repo: https://github.com/abravalheri/validate-pyproject
-  rev: v0.12.2
+  rev: v0.13
   hooks:
   - id: validate-pyproject
 
 - repo: https://github.com/psf/black
-  rev: 23.3.0
+  rev: 23.7.0
   hooks:
   - id: black
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.267
+  rev: v0.0.280
   hooks:
   - id: ruff
     args: [--fix, --exit-non-zero-on-fix]
 
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.9.0
+  rev: v2.10.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
 
 # for docstrings in python codes
 - repo: https://github.com/myint/docformatter
-  rev: v1.7.0
+  rev: v1.7.5
   hooks:
   - id: docformatter
     additional_dependencies: [tomli]
     args: [--in-place]
```

### Comparing `smartdoor-2.0.0.dev1/LICENSE.md` & `smartdoor-2.0.0.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/README.md` & `smartdoor-2.0.0.dev2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -6,44 +6,59 @@
 [![GitHub](https://img.shields.io/github/license/munechika-koyo/cherab_phix)](https://opensource.org/licenses/BSD-3-Clause)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc. with Raspberry Pi.
 
 ## Quick Installation
 ```bash
-$ python -m pip install smartdoor
+python -m pip install smartdoor
 ```
 
 ## Before getting started
 
 ### `smartdoor_host` system
 Smartdoor Host system which serves the web application for NFC key management must be run. Please
 install and deploy it in adavnce. ([see here](https://github.com/munechika-koyo/smartdoor_host)).
 
 ### pigpio library
 `pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance. ([see here](http://abyz.me.uk/rpi/pigpio/download.html))
 
 ## How to use
 
+Almost all the operations are done by the `smartdoor` command. Please see the help message for the
+details:
+```bash
+smartdoor --help
+```
+
 ### 1. Set up the configuration file
 The default configuration file ca be generated by the following command:
 ```bash
 smartdoor config --generate
 ```
 The configuration file is located at `~/.config/smartdoor.toml`. Please edit it according to your environment.
 
-### 2. Run the main program
+### 2. Run the main program for testing
 The main program can be executed by the following command:
 ```bash
 smartdoor start
 ```
-Then, the main program will be run in the foreground. If you want stop the program, press `Ctrl+C`.
+If you want to specify door is locked/unlocked, add `--locked`/`--unlocked` option, by default
+the door is locked.
+
+The main program will be run in the foreground. If you want stop the program, press `Ctrl+C`.
 
 ### 3. Set up the auto start
-The main program can be automatically run by `systemd` service. To register and start the service, execute the following command:
+The main program can be automatically run by `systemd` service. To register the `smartdoor.service`
+to `systemd`, execute the following command:
 ```bash
 smartdoor service --register
 ```
-Then, the service will be registered and started. To stop the service, execute the following command:
+Then, the service will be ready for start. To manually start it, execute the following command:
+```bash
+smartdoor service --start
+```
+
+Please see the help message for other options:
 ```bash
-smartdoor service --stop
+smartdoor service --help
 ```
```

### Comparing `smartdoor-2.0.0.dev1/pyproject.toml` & `smartdoor-2.0.0.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/smartdoor/__init__.py` & `smartdoor-2.0.0.dev2/smartdoor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 try:
     import tomllib
 except ImportError:
     import tomli as tomllib
 
 from .smartdoor import SmartDoor
 
-__version__ = "2.0.0.dev1"
+__version__ = "2.0.0.dev2"
 __all__ = ["SmartDoor"]
 
 
 @click.group(context_settings=dict(help_option_names=["-h", "--help"]))
 @click.version_option(__version__, "-V", "--version")
 def cli():
     """Smartdoor system CLI."""
@@ -138,49 +138,89 @@
             file.write(default_config_path.read_text())
         click.echo(f"generated default config file as {config_path}")
 
     # Show configuation
     elif show:
         click.echo(pformat(config))
     else:
-        click.echo("please specify `--show` or `--generate` option")
+        click.echo(click.get_current_context().get_help())
 
 
 @cli.command()
-@click.option("--register", is_flag=True, help="register service to systemd and start it")
+@click.option("--register", is_flag=True, help="register service to systemd")
 @click.option("--unregister", is_flag=True, help="unregister service from systemd")
 @click.option("--start", is_flag=True, help="start service")
 @click.option("--stop", is_flag=True, help="stop service")
-def service(register: bool, unregister: bool, start: bool, stop: bool):
+@click.option("--restart", is_flag=True, help="restart service")
+@click.option("--status", is_flag=True, help="show service status")
+def service(register: bool, unregister: bool, start: bool, stop: bool, restart: bool, status: bool):
     """Systemd Service tool for SmartDoor system.
 
     If you want to register/unregister smartdoor system to/from systemd, use `--register` or
-    `--unregister` option. If choose `--register` option, smartdoor system will be started.
+    `--unregister` option. If choosing `--register` option, smartdoor system will be ready for start
+    automatically.
+
+    You can also start/stop/restart service by `--start`, `--stop`, `--restart` option. If you want
+    to show service status, use `--status` option.
     """
     if register:
-        service_file = Path(__file__).parent / "smartdoor.service"
-        subprocess.run(
-            ["sudo", "ln", "-s", str(service_file), "/etc/systemd/system/smartdoor.service"]
-        )
-        subprocess.run(["sudo", "systemctl", "daemon-reload"])
-        subprocess.run(["sudo", "systemctl", "enable", "smartdoor.service"])
-        click.echo("registered service to systemd")
+        try:
+            service_file = Path(__file__).parent / "smartdoor.service"
+            subprocess.run(
+                ["sudo", "ln", "-s", str(service_file), "/etc/systemd/system/smartdoor.service"],
+                check=True,
+            )
+            subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
+            subprocess.run(["sudo", "systemctl", "enable", "smartdoor.service"], check=True)
+            click.echo("registered service to systemd")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to register service to systemd")
 
     elif unregister:
-        subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"])
-        subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"])
-        click.echo("unregistered service from systemd")
+        try:
+            subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
+            subprocess.run(["sudo", "systemctl", "disable", "smartdoor.service"], check=True)
+            subprocess.run(["sudo", "rm", "/etc/systemd/system/smartdoor.service"], check=True)
+            subprocess.run(["sudo", "systemctl", "daemon-reload"], check=True)
+            click.echo("unregistered service from systemd")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to unregister service from systemd")
 
     elif start:
-        subprocess.run(["sudo", "systemctl", "start", "smartdoor.service"])
-        click.echo("started service")
+        try:
+            subprocess.run(["sudo", "systemctl", "start", "smartdoor.service"], check=True)
+            click.echo("started service")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to start service")
 
     elif stop:
-        subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"])
-        click.echo("stopped service")
+        try:
+            subprocess.run(["sudo", "systemctl", "stop", "smartdoor.service"], check=True)
+            click.echo("stopped service")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to stop service")
+
+    elif restart:
+        try:
+            subprocess.run(["sudo", "systemctl", "restart", "smartdoor.service"], check=True)
+            click.echo("restarted service")
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to restart service")
+
+    elif status:
+        try:
+            subprocess.run(["sudo", "systemctl", "status", "smartdoor.service"], check=True)
+        except subprocess.CalledProcessError as e:
+            click.echo(e)
+            click.echo("failed to show service status")
 
     else:
-        click.echo("please specify `--register` or `--unregister` option")
+        click.echo(click.get_current_context().get_help())
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `smartdoor-2.0.0.dev1/smartdoor/core/authenticate.py` & `smartdoor-2.0.0.dev2/smartdoor/core/authenticate.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/smartdoor/core/smartlock.py` & `smartdoor-2.0.0.dev2/smartdoor/core/smartlock.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/smartdoor/default_config.toml` & `smartdoor-2.0.0.dev2/smartdoor/default_config.toml`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/smartdoor/logging.conf` & `smartdoor-2.0.0.dev2/smartdoor/logging.conf`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/smartdoor/smartdoor.py` & `smartdoor-2.0.0.dev2/smartdoor/smartdoor.py`

 * *Files identical despite different names*

### Comparing `smartdoor-2.0.0.dev1/PKG-INFO` & `smartdoor-2.0.0.dev2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartdoor
-Version: 2.0.0.dev1
+Version: 2.0.0.dev2
 Summary: Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc.
 Author-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Maintainer-email: Koyo Munechika <munechika.koyo@torus.nr.titech.ac.jp>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -39,45 +39,60 @@
 [![GitHub](https://img.shields.io/github/license/munechika-koyo/cherab_phix)](https://opensource.org/licenses/BSD-3-Clause)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/charliermarsh/ruff)
 
 Smartdoor system including NFC card detecting, key locking/unlocking, turning LED on/off, etc. with Raspberry Pi.
 
 ## Quick Installation
 ```bash
-$ python -m pip install smartdoor
+python -m pip install smartdoor
 ```
 
 ## Before getting started
 
 ### `smartdoor_host` system
 Smartdoor Host system which serves the web application for NFC key management must be run. Please
 install and deploy it in adavnce. ([see here](https://github.com/munechika-koyo/smartdoor_host)).
 
 ### pigpio library
 `pigpio` library enables hardware control for PWM signals. This is the optional library for `smartdoor` package. If you want to use it, please install it in advance. ([see here](http://abyz.me.uk/rpi/pigpio/download.html))
 
 ## How to use
 
+Almost all the operations are done by the `smartdoor` command. Please see the help message for the
+details:
+```bash
+smartdoor --help
+```
+
 ### 1. Set up the configuration file
 The default configuration file ca be generated by the following command:
 ```bash
 smartdoor config --generate
 ```
 The configuration file is located at `~/.config/smartdoor.toml`. Please edit it according to your environment.
 
-### 2. Run the main program
+### 2. Run the main program for testing
 The main program can be executed by the following command:
 ```bash
 smartdoor start
 ```
-Then, the main program will be run in the foreground. If you want stop the program, press `Ctrl+C`.
+If you want to specify door is locked/unlocked, add `--locked`/`--unlocked` option, by default
+the door is locked.
+
+The main program will be run in the foreground. If you want stop the program, press `Ctrl+C`.
 
 ### 3. Set up the auto start
-The main program can be automatically run by `systemd` service. To register and start the service, execute the following command:
+The main program can be automatically run by `systemd` service. To register the `smartdoor.service`
+to `systemd`, execute the following command:
 ```bash
 smartdoor service --register
 ```
-Then, the service will be registered and started. To stop the service, execute the following command:
+Then, the service will be ready for start. To manually start it, execute the following command:
+```bash
+smartdoor service --start
+```
+
+Please see the help message for other options:
 ```bash
-smartdoor service --stop
+smartdoor service --help
 ```
```

