# Comparing `tmp/kuki-0.3.0.tar.gz` & `tmp/kuki-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuki-0.3.0.tar", last modified: Tue Jul  4 16:06:49 2023, max compression
+gzip compressed data, was "kuki-0.9.7.tar", last modified: Tue Jul 25 13:38:34 2023, max compression
```

## Comparing `kuki-0.3.0.tar` & `kuki-0.9.7.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.3.0/LICENSE
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13802 2023-07-04 16:06:49.922429 kuki-0.3.0/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2221 2023-07-03 15:40:17.000000 kuki-0.3.0/README.md
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.920429 kuki-0.3.0/kuki/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.3.0/kuki/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.3.0/kuki/config_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1563 2023-07-04 15:42:52.000000 kuki-0.3.0/kuki/kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1521 2023-07-04 15:42:58.000000 kuki-0.3.0/kuki/ktrl.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3371 2023-06-09 16:35:49.000000 kuki-0.3.0/kuki/kuki.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3313 2023-05-13 05:48:24.000000 kuki-0.3.0/kuki/package_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      279 2023-06-09 16:35:43.000000 kuki-0.3.0/kuki/profile_util.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/kuki/q/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.3.0/kuki/q/cli.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     6406 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/kest.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      175 2023-07-04 15:27:24.000000 kuki-0.3.0/kuki/q/ktrl.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1853 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/kuki.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2177 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/log.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      878 2023-07-03 12:47:22.000000 kuki-0.3.0/kuki/q/path.q
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13261 2023-06-09 16:35:40.000000 kuki-0.3.0/kuki/registry_util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3619 2023-07-04 15:58:02.000000 kuki-0.3.0/kuki/util.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       22 2023-07-04 16:05:26.000000 kuki-0.3.0/kuki/version.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.921429 kuki-0.3.0/kuki.egg-info/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    13802 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/PKG-INFO
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      573 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/SOURCES.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/dependency_links.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/entry_points.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/not-zip-safe
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       17 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/requires.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-04 16:06:49.000000 kuki-0.3.0/kuki.egg-info/top_level.txt
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      486 2023-07-04 16:06:49.922429 kuki-0.3.0/setup.cfg
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.3.0/setup.py
-drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-04 16:06:49.922429 kuki-0.3.0/test/
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.3.0/test/__init__.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.3.0/test/conftest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1399 2023-07-03 12:47:22.000000 kuki-0.3.0/test/test_kest.py
--rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    14435 2023-05-20 06:46:07.000000 kuki-0.3.0/test/test_kuki.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    11357 2023-05-07 13:15:07.000000 kuki-0.9.7/LICENSE
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-25 13:38:34.471388 kuki-0.9.7/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      459 2023-07-20 14:47:33.000000 kuki-0.9.7/README.md
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.469388 kuki-0.9.7/kuki/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:14:38.000000 kuki-0.9.7/kuki/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1176 2023-05-20 06:39:32.000000 kuki-0.9.7/kuki/config_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1375 2023-07-23 05:45:31.000000 kuki-0.9.7/kuki/kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1994 2023-07-19 16:18:20.000000 kuki-0.9.7/kuki/ktrl.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4652 2023-07-22 06:51:24.000000 kuki-0.9.7/kuki/ktrl_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4577 2023-07-22 07:28:15.000000 kuki-0.9.7/kuki/kuki.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4087 2023-07-23 15:13:37.000000 kuki-0.9.7/kuki/package_util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/kuki/q/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-03 12:47:22.000000 kuki-0.9.7/kuki/q/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     4535 2023-07-03 16:51:49.000000 kuki-0.9.7/kuki/q/cli.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     7819 2023-07-15 09:03:13.000000 kuki-0.9.7/kuki/q/kest.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      219 2023-07-19 16:35:57.000000 kuki-0.9.7/kuki/q/ktrl.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1913 2023-07-22 16:08:18.000000 kuki-0.9.7/kuki/q/kuki.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     2187 2023-07-20 15:49:50.000000 kuki-0.9.7/kuki/q/log.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1435 2023-07-15 14:20:22.000000 kuki-0.9.7/kuki/q/path.q
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    18554 2023-07-25 13:34:57.000000 kuki-0.9.7/kuki/registry_util.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     3704 2023-07-19 16:32:47.000000 kuki-0.9.7/kuki/util.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.470388 kuki-0.9.7/kuki.egg-info/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    12044 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/PKG-INFO
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      554 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/SOURCES.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/dependency_links.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       84 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/entry_points.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        1 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/not-zip-safe
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       15 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/requires.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)       10 2023-07-25 13:38:34.000000 kuki-0.9.7/kuki.egg-info/top_level.txt
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      468 2023-07-25 13:38:34.472388 kuki-0.9.7/setup.cfg
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)      315 2023-07-03 15:40:17.000000 kuki-0.9.7/setup.py
+drwxr-xr-x   0 jshinonome  (1000) jshinonome  (1000)        0 2023-07-25 13:38:34.471388 kuki-0.9.7/test/
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.7/test/__init__.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)        0 2023-05-07 13:15:07.000000 kuki-0.9.7/test/conftest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)     1423 2023-07-19 15:39:03.000000 kuki-0.9.7/test/test_kest.py
+-rw-r--r--   0 jshinonome  (1000) jshinonome  (1000)    15810 2023-07-21 15:26:05.000000 kuki-0.9.7/test/test_kuki.py
```

### Comparing `kuki-0.3.0/LICENSE` & `kuki-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kuki-0.3.0/PKG-INFO` & `kuki-0.9.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,33 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.3.0
-Summary: kdb+/q package manager
+Version: 0.9.7
+Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
-Keywords: kdb,q
+Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## K Ultimate pacKage Installer
 
-- use the same registry site as the npm
-- use file `$HOME/.kukirc.json` to configure local registry site and token
-- default local repo: `$HOME/kuki`, use environment variable `KUKIPATH` to overwrite local repo
-- `kuki.json` to maintain package dependencies
-- `kuki_index.json` to maintain indices of all required packages. For a version conflict:
-  - it will use dependency version if it is a dependency
-  - latest version if it is not a dependency
+Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
 
-### Command: kuki
+### Commands
 
-K Ultimate pacKage Installer
+`kuki` includes a set of 3 commands
 
-#### config
+- kuki: _K Ultimate pacKage Installer_, manage q/k packages
+- kest: _K tEST cli_, test q/k codes
+- ktrl: _K conTRoL cli_,control
 
-use format 'field=value'
+### Registry Site
 
-```bash
-kuki --config registry=https://localhost token=some_token
-```
-
-#### init
-
-init kuki.json for a new package
-
-```bash
-kuki --init
-```
-
-#### publish
-
-publish current package to the registry
-
-```bash
-kuki --publish
-```
-
-#### download
-
-download a package from the registry
-
-```bash
-kuki --download dummy
-kuki --download dummy@0.0.1
-```
-
-#### install
-
-install a package to the local repo
-
-```bash
-kuki --install dummy
-kuki --install dummy@0.0.1
-```
-
-#### uninstall
-
-uninstall a package from current working package
-
-```bash
-kuki --uninstall dummy
-```
-
-### Command: kest
-
-K tEST CLI
-
-#### Define Test
-
-- `.kest.Test[description;function]`
-
-#### Setup and Teardown
-
-- `.kest.BeforeAll function`
-- `.kest.AfterAll function`
-- `.kest.BeforeEach function`
-- `.kest.AfterEach function`
-
-#### Using Matchers
-
-- `.kest.ToThrow[functionCall;errorMsg]`
-- `.kest.Match[expect;actual]`
-- `.kest.MatchTable[expect;actual]`
-- `.kest.MatchDict[expect;actual]`
-
-### Command: ktrl
-
-K conTRoL CLI
-
-#### Init ktrl Profile
-
-`ktrl -init [-global|mongodb] profile_name`
-
-locations for profiles
-
-- mongodb: stored in MongoDB
-- global: `$HOME/kuki/_profile`
-- local: `$PWD/profile`
-
-#### Start Process Using ktrl Profile
-
-`ktrl -profile [-global|mongodb] profile_name`
-
-- with `-mongodb`, ktrl will use profiles in MongoDB
-- with `-global`, ktrl will use profiles in global profile directory
-- without `-global|mongodb`, ktrl will use profiles as following priorities:
-  - local directory
-  - global profile directory
-  - MongoDB
-
-#### Config ktrl
-
-`ktrl -config`
-
-Config ktrl includes MongoDB connection details, configuration file path `$HOME/kuki/_config/ktrlrc.json`
+`kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.3.0/kuki/config_util.py` & `kuki-0.9.7/kuki/config_util.py`

 * *Files identical despite different names*

### Comparing `kuki-0.3.0/kuki/kest.py` & `kuki-0.9.7/kuki/kest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 import json
 import logging
 import subprocess
 import sys
 from pathlib import Path
 
-from .util import ENV_DEFAULT, PROCESS_DEFAULT, generate_cmd, generate_options
+from .util import PROFILE_DEFAULT, generate_cmd, generate_process_options
 
 FORMAT = "%(asctime)s %(levelname)s: %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
 logging.basicConfig(level=logging.INFO, format=FORMAT, datefmt=DATE_FORMAT)
 
 logger = logging.getLogger()
 
 kest_path = Path("kest.json")
 
-kest_process_default = PROCESS_DEFAULT.copy()
-
-kest_process_default.pop("blocked")
-kest_process_default.pop("replicate")
-kest_process_default.pop("disable_system_cmd")
-
 KEST_DEFAULT = {
-    "process": kest_process_default,
-    "environment": ENV_DEFAULT,
+    "process": {},
+    "profile": PROFILE_DEFAULT,
 }
 
 
 def kest(args):
     # use kest.json if available
     if "-init" in args:
         # generate kest.json
         if kest_path.exists():
             logger.warn("kest.json already exists, skip...")
             return
         with open(kest_path, "w") as file:
             json.dump(KEST_DEFAULT, file, indent=2)
     else:
         kest_json = load_kest()
-        options = generate_options(args, kest_json.get("process"))
+        options = generate_process_options(args, kest_json.get("process"))
         # generate run command
         options = ["-kScriptType", "kest"] + args + options
 
-        cmd = generate_cmd(options, kest_json.get("environment"))
+        cmd = generate_cmd(options, kest_json.get("profile"))
         logger.info("starting " + cmd)
         try:
             subprocess.run(cmd, shell=True, check=True)
         except subprocess.CalledProcessError:
             exit(1)
```

### Comparing `kuki-0.3.0/kuki/kuki.py` & `kuki-0.9.7/kuki/kuki.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import getpass
 import logging
 
 from . import config_util, package_util, registry_util
 
 FORMAT = "%(asctime)s %(levelname)s: %(message)s"
 DATE_FORMAT = "%Y-%m-%d %H:%M:%S"
 
@@ -29,71 +30,95 @@
     help="config kukirc, use format 'field=value'",
 )
 
 group.add_argument(
     "-d",
     "--download",
     type=str,
-    help="download a kdb package of latest version, use '@' to specify a version",
+    help="download a q/k package of latest version, use '@' to specify a version",
 )
 
 
 group.add_argument(
     "-i",
     "--install",
     nargs="*",
-    help="install a kdb package of latest version, use '@' to specify a version",
+    help="install a q/k package of latest version, use '@' to specify a version",
 )
 
 group.add_argument(
     "--init",
     action="store_true",
     default=False,
-    help="init a kdb package",
+    help="init a q/k package",
 )
 
 group.add_argument(
     "--login",
     action="store_true",
     default=False,
     help="login to registry",
 )
 
 group.add_argument(
     "-p",
     "--publish",
     action="store_true",
     default=False,
-    help="publish a kdb package using kuki.json",
+    help="publish a q/k package using kuki.json",
+)
+
+group.add_argument(
+    "--unpublish",
+    type=str,
+    help="unpublish a q/k package",
+)
+
+
+group.add_argument(
+    "--pack",
+    action="store_true",
+    default=False,
+    help="pack a q/k package using kuki.json",
 )
 
 group.add_argument(
     "-s",
     "--search",
     type=str,
-    help="search a kdb package",
+    help="search a q/k package",
 )
 
 
 group.add_argument(
     "-u",
     "--uninstall",
     nargs="+",
-    help="uninstall a kdb package, use '@' to specify a version",
+    help="uninstall a q/k package, use '@' to specify a version",
 )
 
 group.add_argument(
     "-v",
     "--version",
     choices=["patch", "minor", "major"],
     help="roll up version(patch, minor, major)",
 )
 
 
-def kuki(args):
+parser.add_argument(
+    "-g",
+    "--global",
+    action="store_true",
+    default=False,
+    dest="globalMode",
+    help="enable global mode",
+)
+
+
+def kuki(args: argparse.Namespace):
     if args.config:
         for arg in args.config:
             if "=" in arg:
                 field, value = arg.split("=")
                 allowed_config_fields = ["token", "registry"]
                 if field in allowed_config_fields:
                     config_util.update_config(field, value)
@@ -102,33 +127,50 @@
                     logger.info("allowed config fields " + ",".join(allowed_config_fields))
             else:
                 logger.warning("requires to use '=' to separate field and value")
     elif args.init:
         package_util.init()
     elif args.adduser:
         user = input("Username: ")
-        password = input("Password: ")
+        password = getpass.getpass("Password: ")
+        confirmed_pass = getpass.getpass("Confirm password: ")
+        if confirmed_pass != password:
+            logger.info("Password doesn't match, Try again")
+            return
         email = input("Email: ")
-        registry_util.add_user(user, password, email)
+        logger.info("About to register '{}' with '{}'".format(user, password))
+        proceed = input("Is this OK? (yes/no) ").strip()
+        if proceed.lower() == "yes":
+            registry_util.add_user(user, password, email)
+        else:
+            logger.info("Abort registering '{}'".format(user))
     elif args.login:
         user = input("Username: ")
-        password = input("Password: ")
+        password = getpass.getpass("Password: ")
         registry_util.login(user, password)
     elif args.search:
         registry_util.search_package(args.search)
     elif args.download:
         registry_util.download_entry(args.download)
+    elif args.unpublish:
+        registry_util.unpublish_package(args.unpublish)
     else:
-        if not package_util.exits():
+        if args.globalMode:
+            if isinstance(args.install, list):
+                registry_util.install_packages(args.install, False, True)
+                registry_util.dump_global_index()
+        elif not package_util.exits():
             logger.error("kuki.json not found, use 'kuki --init' to init the package first")
             return
         elif args.version:
             package_util.roll_up_version(args.version)
         elif args.publish:
             registry_util.publish_entry()
+        elif args.pack:
+            registry_util.pack_entry()
         elif isinstance(args.install, list):
             registry_util.install_entry(args.install)
         elif args.uninstall:
             registry_util.uninstall_entry(args.uninstall)
 
 
 def main():
```

### Comparing `kuki-0.3.0/kuki/package_util.py` & `kuki-0.9.7/kuki/package_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,81 @@
 import json
 import logging
 import os
+import re
 from pathlib import Path
 from typing import Dict, List, TypedDict
 
 logger = logging.getLogger()
 config_file = "kuki.json"
 index_file = "kuki_index.json"
 readme_file = "README.md"
 
 package_path = Path.cwd()
 readme_path = Path(readme_file)
+src_path = Path("src")
 package_config_path = Path(config_file)
 package_include_path = Path(".kukiinclude")
 package_index_path = Path(index_file)
 
 
 class Kuki(TypedDict):
     name: str
     version: str
     description: str
     author: str
     git: str
     dependencies: Dict[str, str]
 
 
-def generate_json(name: str, description="", author="", git=""):
+def generate_json(name: str, description="", author="", git="", package_type="q"):
     if package_config_path.exists():
         overwrite = input("kuki.json already exists, overwrite: (yes/No) ").strip()
         if not overwrite or not overwrite.lower() in ["yes"]:
             return
     kuki: Kuki = {
         "name": name,
         "version": "0.0.1",
         "description": description,
         "author": author,
         "git": git,
+        "type": package_type,
         "dependencies": {},
     }
     kuki_json = json.dumps(kuki, indent=2)
     logger.info("About to write to {}".format(package_config_path))
     logger.info("\n" + kuki_json)
     proceed = input("Is this OK? (YES/no) ").strip()
     if not proceed or proceed.lower() == "yes":
         dump_kuki(kuki)
         readme_path.touch()
+        readme_path.write_text("# {name}\n\n- author: {author}\n- git: {git}\n".format(**kuki))
+        package_index_path.write_text("{}")
+        src_path.mkdir(parents=True, exist_ok=True)
 
 
 def init():
     dir = os.path.basename(os.getcwd())
-    package = input("package name: ({}) ".format(dir)).strip()
+    package = input("package name: ({}) ".format(dir.lower())).strip()
     if not package:
-        package = dir
+        package = dir.lower()
+
+    is_valid_name(package)
+
     description = input("description: ").strip()
     author = input("author: ").strip()
     git = input("git repository: ").strip()
+    package_type = input("package type: (q)").strip()
+    if not package_type:
+        package_type = "q"
+    if package_type not in ["q", "k", "k9"]:
+        logger.error("only support q, k, or k9 package type")
+        return
 
-    generate_json(package, description, author, git)
+    generate_json(package, description, author, git, package_type)
 
 
 def dump_kuki(kuki: Kuki):
     with open(package_config_path, "w") as file:
         file.write(json.dumps(kuki, indent=2))
 
 
@@ -92,15 +107,15 @@
     if package_config_path.exists():
         return json.loads(package_config_path.read_text())
     else:
         return {}
 
 
 def load_include() -> List[str]:
-    includes = set(["src/*", "lib/*", config_file, readme_file])
+    includes = set(["src/*", "cfg/*", config_file, index_file, readme_file])
     if package_include_path.exists():
         with open(package_include_path, "r") as file:
             while line := file.readline():
                 if line.strip() != "":
                     includes.add(line.strip())
     return includes
 
@@ -117,7 +132,13 @@
     else:
         return {}
 
 
 def dump_pkg_index(kuki_index: Dict[str, Kuki]):
     with open(package_index_path, "w") as file:
         json.dump(kuki_index, file, indent=2)
+
+
+def is_valid_name(name: str) -> bool:
+    if re.fullmatch(r"(@[a-z-]+/)?[a-z-]+", name) is None:
+        logger.error("only allows lower cases(a-z) and hyphen(-) as the package name")
+        exit(1)
```

### Comparing `kuki-0.3.0/kuki/q/cli.q` & `kuki-0.9.7/kuki/q/cli.q`

 * *Files identical despite different names*

### Comparing `kuki-0.3.0/kuki/q/kest.q` & `kuki-0.9.7/kuki/q/kest.q`

 * *Files 16% similar despite different names*

```diff
@@ -23,36 +23,79 @@
     -2 "duplicate description: '", description, "' in ", -3!.kest.currentFile;
     exit 1;
   ];
   `.kest.tests upsert enlist (.kest.currentFile;description;`Test;function);
  };
 
 .kest.ToThrow:{[functionCall;errorMsg]
-  .kest.Match[errorMsg;@[value;functionCall;{x}]]
+  .kest.match[errorMsg;@[value;functionCall;{x}];"Error Msg "]
  };
 
-.kest.Match:{[expect;actual]
-  if[not expect~actual;
-    msg: "\n" sv (
-      "  Mismatch";
-      "    Expected: ", -3!expect;
-      "    Received: ", -3!actual
-    );
-    -2 .kest.getMsgByStyle[`red;msg];
-    'msg;
+.kest.raise:{[msg] -2 .kest.getMsgByStyle[`red;msg];'msg};
+
+.kest.match:{[expect;actual;item]
+  if[expect~actual;
+    :1b;
   ];
-  :1b;
+  msg: "\n" sv (
+    "  ",item,"Mismatch";
+    "    Expected: ", -3!expect;
+    "    Received: ", -3!actual
+  );
+  .kest.raise msg;
+ };
+
+.kest.Match:{[expect;actual]
+  .kest.match[expect;actual;""]
  };
 
-.kest.MatchTable:{[expectTable;actualTable]
 
+.kest.getConsoleFormat:{.Q.S[system"c";0j;x]};
+
+.kest.matchTable:{[expectTable;actualTable;filter;item]
+  if[expectTable~actualTable;:1b];
+  missing:filter expectTable except actualTable;
+  extra:filter actualTable except expectTable;
+  msg: "\n" sv(
+    (enlist "  ",item,"Mismatch"),
+    ((2 8#" "),
+      {"    (",x,") "}'[(,/)(count each (missing;extra))#'"+-"]),'
+      .kest.getConsoleFormat[missing uj extra]
+  );
+  .kest.raise msg;
  };
 
-.kest.MatchDict:{[expectDict;actualDict]
+.kest.MatchTable:{[expectTable;actualTable]
+  if[not all isTable:.Q.qt each (expectTable;actualTable);
+    msg:"not a table - ",(-3!`expectTable`actualTable where not isTable);
+    .kest.raise msg;
+  ];
+  if[expectTable~actualTable;
+    :1b;
+  ];
+  .kest.match[cols expectTable;cols actualTable;"Column "];
+  .kest.matchTable[0!meta expectTable;0!meta actualTable;(::);"Meta "];
+  :.kest.matchTable[0!expectTable;0!actualTable;(5 sublist);"Record(show <=5 diff) "];
+ };
 
+.kest.MatchDict:{[expectDict;actualDict]
+  if[not all isDict:99h=type each(expectDict;actualDict);
+    msg:"not a dict - ",(-3!`expectDict`actualDict where not isDict);
+    .kest.raise msg;
+  ];
+  if[expectDict~actualDict;
+    :1b;
+  ];
+  .kest.match[key expectDict;key actualDict;"Key "];
+  .kest.matchTable[
+    ([]k:key expectDict;v:value expectDict);
+    ([]k:key actualDict;v:value actualDict);
+    (::);
+    "Dict "
+  ];
  };
 
 / output format
 / collected * items
 / PASSED
 / FAILED
 / test file name
@@ -205,8 +248,9 @@
 .cli.Symbol[`testOutputFile;`;"write test results to a file"];
 .cli.String[`testPattern;"*";"run only tests with a name that matches the pattern"];
 .cli.Symbol[`testFile;`;"run specific test file"];
 .cli.SetName["K tEST CLI"];
 .cli.Parse[];
 
 .kest.startupPath:.path.Cwd[];
+.kuki.SetPath[.path.ToString .cli.args`testRoot];
 .kest.run[hsym .cli.args`testRoot];
```

### Comparing `kuki-0.3.0/kuki/q/kuki.q` & `kuki-0.9.7/kuki/q/kuki.q`

 * *Files 6% similar despite different names*

```diff
@@ -7,30 +7,33 @@
     .kuki.appendSlash[path],subPaths;
     (,/)(.kuki.appendSlash each enlist[path],-1_subPaths),-1#subPaths
   ]
  };
 
 .kuki.rootDir:{kukiRoot:getenv`KUKIPATH;$[count kukiRoot;kukiRoot;.kuki.joinPath[getenv`HOME;("kuki")]]}[];
 
-
-.kuki.getRealPath:{[modulePath]
-  first @[system;"realpath ", modulePath;{'y, " - No such file or directory"}[;modulePath]]
+.kuki.getRealPath:{[path]
+  first @[system;"realpath ", path;{'y, " - No such file or directory"}[;path]]
  };
 
-.kuki.appendDotQ:{ x,$[x like "*.q";"";".q"] };
+.kuki.appendDotQ:{ x,$[any x like/: ("*.q";"*.k");"";".q"] };
 
 .kuki.importModule:{[modulePath]
   realPath: .kuki.getRealPath modulePath;
   if[realPath in .kuki.importedModules;:(::)]
   system"l ", realPath;
   .kuki.importedModules,:realPath;
  };
 
+.kuki.path:{x,:$[x like "/src";"";"/src"]}getenv`PWD;
+
+.kuki.SetPath:{.kuki.path:x};
+
 .kuki.importLocal:{[path;module]
-  if[0=count path;path:getenv`PWD;path,:$[path like "/src";"";"/src"]];
+  if[0=count path;path:.kuki.path];
   modulePath: .kuki.joinPath[path;.kuki.appendDotQ module];
   .kuki.importModule modulePath
  };
 
 .kuki.index:.j.k (,/) @[read0;`:kuki_index.json;{"{}"}];
 
 .kuki.importGlobal:{[module]
@@ -45,15 +48,15 @@
 // local import - import {"./[folder/]/module"}
 // module doesn't include .q
 import:{[moduleFunc]
   if[100h<>type moduleFunc;'"requires format {\"module\"} for import"];
   module: moduleFunc[];
   path: first -3#value moduleFunc;
   path: 1_string first ` vs hsym `$path;
-  $[module like "./*"; .kuki.importLocal[path;module];.kuki.importGlobal[module]]
+  $[any module like/: ("./*";"../*"); .kuki.importLocal[path;module];.kuki.importGlobal[module]]
  };
 
 import {"./log"};
 import {"./cli"};
 import {"./path"};
 
 import {"./",first .Q.opt[.z.x][`kScriptType]};
```

### Comparing `kuki-0.3.0/kuki/q/log.q` & `kuki-0.9.7/kuki/q/log.q`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,22 @@
   .log.Info:.log.log["INFO "];
   .log.Warning:.log.log["WARN "];
   .log.Error:.log.log["ERROR"];
   .log.SetLogLevel .log.level;
  };
 
 .log.SetStdLogFile:{[filepath]
-  h:hopen filepath;
+  h:hopen hsym filepath;
   .log.stdHandle:h;
   .log.errHandle:h;
   .log.refreshLogMethod[];
  };
 
 .log.SetErrLogFile:{[filepath]
-  h:hopen filepath;
+  h:hopen hsym filepath;
   .log.errHandle:h;
   .log.refreshLogMethod[];
  };
 
 .log.SetConsoleSize:{[consoleSize]
   system"c ", " " sv string $[-6 -6h~type each consoleSize;consoleSize;0 0i] | system"c";
  };
```

### Comparing `kuki-0.3.0/kuki/q/path.q` & `kuki-0.9.7/kuki/q/path.q`

 * *Files 19% similar despite different names*

```diff
@@ -32,7 +32,30 @@
 .path.Glob:{[path;pattern]
   :?[.path.Walk[path];enlist(like;`file;pattern);0b;()];
  };
 
 .path.Home:{hsym `$getenv`HOME};
 
 .path.Cwd:{hsym `$first system"pwd"};
+
+.path.appendSlash:{[path]
+  .kuki.appendSlash path
+ };
+
+// same as .kuki.getRealPath
+.path.GetRealPath:{[path]
+  .kuki.getRealPath .path.ToString path
+ };
+
+// same as .kuki.joinPath
+.path.JoinPath:{[path;subPaths]
+  path:.path.ToString path;
+  subPaths:$[type[subPaths] in 0 10h;subPaths;.path.ToString each subPaths];
+  .path.ToHsym .kuki.joinPath[.path.ToString path;subPaths]
+ };
+
+.path.GetRelativePath:{[pathFunc]
+  targetPath: pathFunc[];
+  path: first -3#value pathFunc;
+  path: 1_string first ` vs hsym `$path;
+  .path.JoinPath[path;targetPath]
+ };
```

### Comparing `kuki-0.3.0/kuki/registry_util.py` & `kuki-0.9.7/kuki/registry_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,26 @@
 import os
 import shutil
 import tarfile
 from pathlib import Path
 from typing import Dict, List, TypedDict
 
 import requests
+import urllib3
 from requests.auth import HTTPBasicAuth
 
 from . import config_util, package_util
 
+urllib3.disable_warnings()
+
 logger = logging.getLogger()
 config = config_util.load_config()
-registry = config.get("registry", "http://0.0.0.0:4873/")
+registry = config.get("registry", "https://kuki.ninja/")
 token = config.get("token", "")
+user = config.get("user", "")
 
 global_cache_dir = Path.joinpath(config_util.global_kuki_root, "_cache")
 global_index_path = Path.joinpath(config_util.global_kuki_root, ".index")
 
 kuki_json = package_util.load_kuki()
 
 if global_cache_dir.exists() and not global_cache_dir.is_dir():
@@ -36,14 +40,15 @@
 
 
 class Metadata(TypedDict):
     name: str
     version: str
     dist: any
     dependencies: any
+    type: str
 
 
 def load_global_index() -> Dict[str, package_util.Kuki]:
     if global_index_path.exists():
         with open(global_index_path, "r") as file:
             return json.load(file)
     else:
@@ -52,41 +57,45 @@
 
 global_index = load_global_index()
 
 
 def add_user(user: str, password: str, email: str):
     payload = {"name": user, "password": password, "email": email}
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
-    res = requests.put(user_url + user, json.dumps(payload), headers=headers)
+    res = requests.put(user_url + user, json.dumps(payload), headers=headers, verify=False)
 
     if res.status_code == 201:
         logger.info("the user '{}' has been added".format(user))
         token = res.json()["token"]
         config_util.update_config("token", token)
+        config_util.update_config("user", user)
     else:
         logger.error("failed to add user: " + user)
         logger.error("status code: {}, error: {}".format(res.status_code, res.json()["error"]))
 
 
 def login(user: str, password: str):
     basic_auth = HTTPBasicAuth(user, password)
     payload = {"name": user, "password": password}
     headers = {"Accept": "application/json", "Content-Type": "application/json"}
-    res = requests.put(user_url + user, json.dumps(payload), headers=headers, auth=basic_auth)
+    res = requests.put(
+        user_url + user, json.dumps(payload), headers=headers, auth=basic_auth, verify=False
+    )
     if res.status_code == 201:
         logger.info("you are authenticated as '{}'".format(user))
         token = res.json()["token"]
         config_util.update_config("token", token)
+        config_util.update_config("user", user)
     else:
         logger.error("failed to authenticated as '{}'".format(user))
         logger.error("status code: {}, error: {}".format(res.status_code, res.json()["error"]))
 
 
 def search_package(package: str):
-    res = requests.get(search_url.format(package))
+    res = requests.get(search_url.format(package), verify=False)
     logger.info(
         "{:20.20} | {:20.20} | {:20.20} | {:10.10} | {:10.10} | {:10.10}".format(
             "NAME", "DESCRIPTION", "AUTHOR", "DATE", "VERSION", "KEYWORDS"
         )
     )
     for obj in res.json()["objects"]:
         pkg = obj["package"]
@@ -98,54 +107,97 @@
                 pkg["time"]["modified"],
                 pkg["dist-tags"]["latest"],
                 " ".join(pkg.get("keywords", "")),
             )
         )
 
 
+def get_publisher(pkg_name: str) -> str:
+    headers = {
+        "Authorization": "Bearer {}".format(token),
+    }
+    res = requests.get(registry + pkg_name, headers=headers, verify=False)
+    if res.status_code == 404:
+        return ""
+    else:
+        pkg = res.json()
+        latest_version = pkg["dist-tags"]["latest"]
+        return pkg["versions"][latest_version]["publisher"]
+
+
 def publish_entry():
     try:
+        if not user:
+            logger.error(
+                "run 'kuki --adduser' or 'kuki --login' first and then publish the package"
+            )
+            return
         publish_package()
     except Exception as e:
         logger.error("failed to publish")
         logger.error(e)
 
 
-def publish_package():
-    kuki = package_util.load_kuki()
-    pkg_name = kuki.get("name")
-    version = kuki.get("version")
+def pack_package(pkg_name: str, version: str):
     logger.info("📦  {}@{}".format(pkg_name, version))
 
     includes = package_util.load_include()
     tar_name = get_tar_name(pkg_name, version)
-    tar = tarfile.open(tar_name, "w:gz")
 
     files = set([])
     for pattern in includes:
         for file in glob.glob(pattern):
             files.add(file)
 
     logger.info("=== Tarball Contents === ")
 
+    tar = tarfile.open(tar_name, "w:gz")
     tar_unpacked_size = 0
     for file in files:
         size = os.path.getsize(file)
         logger.info("{:10d} | {:30.30}".format(size, os.path.basename(file)))
         tar_unpacked_size += size
         tar.add(file)
-
     tar.close()
 
     tar_packed_size = os.path.getsize(tar_name)
     logger.info("=== Tarball Details === ")
     logger.info("filename:      " + tar_name)
     logger.info("package size:  {}".format(tar_packed_size))
     logger.info("unpacked size: {}".format(tar_unpacked_size))
     logger.info("total files:   {}".format(len(files)))
+
+    return tar_name, tar_packed_size
+
+
+def pack_entry():
+    try:
+        kuki = package_util.load_kuki()
+        pkg_name = kuki.get("name")
+        version = kuki.get("version")
+        pack_package(pkg_name, version)
+    except Exception as e:
+        logger.error("failed to pack")
+        logger.error(e)
+
+
+def publish_package():
+    kuki = package_util.load_kuki()
+    pkg_name = kuki.get("name")
+    version = kuki.get("version")
+
+    publisher = get_publisher(pkg_name)
+    if publisher and publisher != user:
+        logger.error("not allowed to publish to other user's package")
+        return
+
+    package_util.is_valid_name(pkg_name)
+
+    tar_name, tar_packed_size = pack_package(pkg_name, version)
+
     logger.info("publishing to {} with tag latest and default access".format(registry))
 
     headers = {
         "Accept": "application/json",
         "Content-Type": "application/json",
         "Authorization": "Bearer {}".format(token),
     }
@@ -169,14 +221,15 @@
         "readme": package_util.load_readme(),
         "versions": {
             version: {
                 "_id": "{}@{}".format(pkg_name, version),
                 "name": pkg_name,
                 "description": kuki.get("package", ""),
                 "author": {"name": kuki.get("author", "unknown")},
+                "publisher": user,
                 "version": version,
                 "readme": package_util.load_readme(),
                 "dependencies": kuki.get("dependencies", {}),
                 "dist": {
                     "shasum": shasum.hexdigest(),
                     "tarball": "{}{}/-/{}".format(registry, pkg_name, tar_name),
                 },
@@ -186,21 +239,107 @@
             tar_name: {
                 "content_type": "application/octet-stream",
                 "data": tar_base64.decode("ascii"),
                 "length": tar_packed_size,
             },
         },
     }
-    res = requests.put(registry + pkg_name, data=json.dumps(data), headers=headers)
+    res = requests.put(registry + pkg_name, data=json.dumps(data), headers=headers, verify=False)
     if res.status_code != 201:
         raise Exception(
             "failed to publish package '{}' with error: {}".format(pkg_name, res.json()["error"])
         )
 
 
+def unpublish_package(pkg_id: str):
+    pkg_name, version = (pkg_id if "@" in pkg_id else pkg_id + "@").split("@")
+
+    headers = {
+        "Authorization": "Bearer {}".format(token),
+    }
+
+    res = requests.get(registry + pkg_name, headers=headers, verify=False)
+    pkg: dict = res.json()
+    if res.status_code != 200:
+        raise Exception(pkg.get("error"))
+    dist_tags: Dict[str, str] = pkg["dist-tags"]
+    latest_version = dist_tags["latest"]
+    publisher = pkg["versions"][latest_version]["publisher"]
+    if user != publisher:
+        logger.error("not allowed to unpublish other user's package")
+        return
+    all_version = pkg.get("versions", {})
+    only_version = len(all_version) == 1
+    no_version = len(all_version) == 0
+
+    if not version or no_version or (only_version and version in all_version):
+        logger.info("unpublishing package '{}'".format(pkg_name))
+        res = requests.delete(
+            registry + pkg_name + "/-rev/" + pkg.get("_rev"),
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        logger.info("successfully unpublish package '{}'".format(pkg_name))
+    else:
+        logger.info("unpublishing package '{}@{}'".format(pkg_name, version))
+        if version not in all_version:
+            logger.error("no version:{} available".format(version))
+            return
+        dist = all_version[version]["dist"]
+        all_version.pop(version)
+
+        for tag in list(dist_tags.keys()):
+            if dist_tags[tag] == version:
+                dist_tags.pop(tag)
+        if latest_version == version:
+            dist_tags["latest"] = max(all_version)
+        pkg.pop("_revisions", None)
+        pkg.pop("_attachments", None)
+        pkg["dist-tags"] = dist_tags
+        pkg["versions"] = all_version
+        res = requests.put(
+            registry + pkg_name + "/-rev/" + pkg.get("_rev"),
+            json=pkg,
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        new_pkg: dict = requests.get(registry + pkg_name, headers=headers, verify=False).json()
+        tarball_url = dist["tarball"]
+        res = requests.delete(
+            tarball_url + "/-rev/" + new_pkg.get("_rev"),
+            headers=headers,
+            verify=False,
+        )
+        if res.status_code != 201:
+            raise Exception(
+                "failed to unpublish package '{}' with error: {}, status code: {}".format(
+                    pkg_name,
+                    res.json()["error"],
+                    res.status_code,
+                )
+            )
+        logger.info("successfully unpublishing package '{}@{}'".format(pkg_name, version))
+
+
 def get_tar_name(name: str, version: str):
     return "{}-v{}.tgz".format(name, version)
 
 
 def get_pkg_path(name: str, version: str):
     return Path.joinpath(config_util.global_kuki_root, name, version)
 
@@ -211,22 +350,24 @@
 
 def get_metadata(name: str) -> Metadata:
     pkg_name, version = (name if "@" in name else name + "@").split("@")
     headers = {
         "Authorization": "Bearer {}".format(token),
     }
     if not version:
-        res = requests.get(registry + name, headers=headers)
+        res = requests.get(registry + name, headers=headers, verify=False)
         res_json = res.json()
         if res.status_code != 200:
             raise Exception(res_json.get("error"))
         version: str = res_json["dist-tags"]["latest"]
         metadata = res_json["versions"][version]
     else:
-        res = requests.get("{}{}/{}".format(registry, pkg_name, version), headers=headers)
+        res = requests.get(
+            "{}{}/{}".format(registry, pkg_name, version), headers=headers, verify=False
+        )
         metadata = res.json()
         if res.status_code != 200:
             raise Exception(metadata.get("error"))
     return metadata
 
 
 def is_cached(tar_name: str) -> bool:
@@ -255,15 +396,15 @@
     tar_name = os.path.basename(tar_url)
     cached_filepath = get_cached_filepath(tar_name)
     logger.info("download package '{}'".format(tar_name))
     if not is_cached(tar_name):
         headers = {
             "Authorization": "Bearer {}".format(token),
         }
-        res = requests.get(tar_url, headers=headers)
+        res = requests.get(tar_url, headers=headers, verify=False)
         if len(res.content) > 0:
             with open(cached_filepath, "wb") as file:
                 file.write(res.content)
         else:
             raise Exception("empty tar file - " + tar_name)
     return cached_filepath
 
@@ -275,54 +416,71 @@
         package_util.dump_kuki(kuki_json)
         package_util.dump_pkg_index(package_index)
         dump_global_index()
     except Exception as e:
         logger.error("failed to install packages with error: {}".format(e))
 
 
-def install_packages(pkgs: List[str], skip_updating_pkg_index=True):
+def install_packages(pkgs: List[str], skip_updating_pkg_index=True, globalMode=False):
+    package_type = kuki_json.get("type", "q")
+
+    if package_type == "k":
+        allow_package_types = ["k"]
+    elif package_type == "k9":
+        allow_package_types = ["k9"]
+    else:
+        allow_package_types = ["q", "k"]
+
     for pkg in pkgs:
         if skip_updating_pkg_index:
             logger.info("install dependency package '{}'".format(pkg))
         else:
             logger.info("install package '{}'".format(pkg))
         metadata = get_metadata(pkg)
+
+        if not metadata.get("type") in allow_package_types and not globalMode:
+            logger.error("")
+
         name = metadata["name"]
-        if name == kuki_json["name"]:
+        if not globalMode and name == kuki_json["name"]:
             logger.warning("shouldn't install itself, skip...")
             return
+
         version = metadata["version"]
         pkg_id = get_pkg_id(metadata)
 
-        if not skip_updating_pkg_index:
+        if not skip_updating_pkg_index and not globalMode:
             kuki_json["dependencies"][name] = version
 
-        if name in package_index and version != package_index[name]["version"]:
-            logger.info("current '{}@{}' exists".format(name, package_index[name]["version"]))
-            if name in kuki_json["dependencies"]:
-                version = kuki_json["dependencies"][name]
-                logger.warning(
-                    "{} is a dependency package, force to use version {}".format(name, version)
-                )
-            elif newer_than(version, package_index[name]["version"]):
-                logger.warning("use newer '{}@{}'".format(name, version))
-            else:
-                logger.warning("skip outdated '{}@{}'".format(name, version))
-                continue
+        if not globalMode:
+            if name in package_index and version != package_index[name]["version"]:
+                logger.info("current '{}@{}' exists".format(name, package_index[name]["version"]))
+                if name in kuki_json["dependencies"]:
+                    version = kuki_json["dependencies"][name]
+                    logger.warning(
+                        "{} is a dependency package, force to use version {}".format(name, version)
+                    )
+                elif newer_than(version, package_index[name]["version"]):
+                    logger.warning("use newer '{}@{}'".format(name, version))
+                else:
+                    logger.warning("skip outdated '{}@{}'".format(name, version))
+                    continue
 
-        package_index[name] = metadata
+            package_index[name] = metadata
 
         if pkg_id in global_index and name in package_index:
             logger.warning("{} is already installed, skip...".format(pkg_id))
             continue
         if pkg_id not in global_index:
-            install_package(metadata)
             # global index uses package id as keys, package index uses package name as keys
             global_index[pkg_id] = metadata
-            install_packages([k + "@" + v for k, v in metadata["dependencies"].items()])
+            install_packages(
+                [k + "@" + v for k, v in metadata["dependencies"].items()], True, globalMode
+            )
+            install_package(metadata)
 
 
 def install_package(metadata: Metadata):
     pkg_filepath = download_package(metadata)
     pkg_path = get_pkg_path(metadata["name"], metadata["version"])
     # already exists
     if pkg_path.exists() and pkg_path.is_dir():
```

### Comparing `kuki-0.3.0/kuki/util.py` & `kuki-0.9.7/kuki/util.py`

 * *Files 9% similar despite different names*

```diff
@@ -35,29 +35,31 @@
     "disable_system_cmd": 0,
     "replicate": "",
     "tls": "plain",
     "blocked": False,
 }
 
 
-ENV_DEFAULT = {
+PROFILE_DEFAULT = {
     # source before running
     "envPath": "",
     "binary": "q",
     # q or k
     "binaryType": "q",
     "binaryHome": "",
     "licenseDir": "",
 }
 
 
-def generate_options(args: List[str], process_cfg: dict[str, str]) -> List[str]:
+def generate_process_options(args: List[str], process_cfg: dict[str, str]) -> List[str]:
     system_args = list(filter(lambda arg: arg[0] == "-" and len(arg) == 2, args))
     cmd = []
     for key, value in process_cfg.items():
+        if key not in CMD_OPTION_MAP:
+            continue
         option = "-" + CMD_OPTION_MAP.get(key)
         # skip command line specified process configuration
         # command line options overwrite kest.json
         if option in system_args:
             continue
 
         if key == "port":
@@ -98,20 +100,20 @@
         if binary_type == "q":
             if env_cfg.get("envPath"):
                 cmd.append("source " + env_cfg.get("envPath"))
             if env_cfg.get("binaryHome"):
                 cmd.append("export QHOME='{}'".format(env_cfg.get("binaryHome")))
             if env_cfg.get("licenseDir"):
                 cmd.append("export QLIC='{}'".format(env_cfg.get("licenseDir")))
-            if "binary" in env_cfg:
-                cmd.append(" ".join([env_cfg.get("binary"), str(q_path), *options]))
+            if env_cfg.get("binary"):
+                cmd.append(" ".join([env_cfg.get("binary", "q"), str(q_path), *options]))
             else:
                 raise Exception("missing binary configuration")
         elif binary_type == "k":
             if env_cfg.get("envPath"):
                 cmd.append("source " + env_cfg.get("envPath"))
-            if "binary" in env_cfg:
-                cmd.append(" ".join([env_cfg.get("binary"), str(k_path), *options]))
+            if env_cfg.get("binary"):
+                cmd.append(" ".join([env_cfg.get("binary", "k"), str(k_path), *options]))
             else:
                 raise Exception("missing binary configuration")
             raise Exception("k is not support yet")
     return ";".join(cmd)
```

### Comparing `kuki-0.3.0/kuki.egg-info/PKG-INFO` & `kuki-0.9.7/kuki.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,134 +1,33 @@
 Metadata-Version: 2.1
 Name: kuki
-Version: 0.3.0
-Summary: kdb+/q package manager
+Version: 0.9.7
+Summary: K Ultimate pacKage Installer
 Author: Jo Shinonome
 License: Apache-2.0
-Keywords: kdb,q
+Keywords: q,k
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ## K Ultimate pacKage Installer
 
-- use the same registry site as the npm
-- use file `$HOME/.kukirc.json` to configure local registry site and token
-- default local repo: `$HOME/kuki`, use environment variable `KUKIPATH` to overwrite local repo
-- `kuki.json` to maintain package dependencies
-- `kuki_index.json` to maintain indices of all required packages. For a version conflict:
-  - it will use dependency version if it is a dependency
-  - latest version if it is not a dependency
+Refer to [wiki](https://github.com/jshinonome/kuki/wiki) for documentations.
 
-### Command: kuki
+### Commands
 
-K Ultimate pacKage Installer
+`kuki` includes a set of 3 commands
 
-#### config
+- kuki: _K Ultimate pacKage Installer_, manage q/k packages
+- kest: _K tEST cli_, test q/k codes
+- ktrl: _K conTRoL cli_,control
 
-use format 'field=value'
+### Registry Site
 
-```bash
-kuki --config registry=https://localhost token=some_token
-```
-
-#### init
-
-init kuki.json for a new package
-
-```bash
-kuki --init
-```
-
-#### publish
-
-publish current package to the registry
-
-```bash
-kuki --publish
-```
-
-#### download
-
-download a package from the registry
-
-```bash
-kuki --download dummy
-kuki --download dummy@0.0.1
-```
-
-#### install
-
-install a package to the local repo
-
-```bash
-kuki --install dummy
-kuki --install dummy@0.0.1
-```
-
-#### uninstall
-
-uninstall a package from current working package
-
-```bash
-kuki --uninstall dummy
-```
-
-### Command: kest
-
-K tEST CLI
-
-#### Define Test
-
-- `.kest.Test[description;function]`
-
-#### Setup and Teardown
-
-- `.kest.BeforeAll function`
-- `.kest.AfterAll function`
-- `.kest.BeforeEach function`
-- `.kest.AfterEach function`
-
-#### Using Matchers
-
-- `.kest.ToThrow[functionCall;errorMsg]`
-- `.kest.Match[expect;actual]`
-- `.kest.MatchTable[expect;actual]`
-- `.kest.MatchDict[expect;actual]`
-
-### Command: ktrl
-
-K conTRoL CLI
-
-#### Init ktrl Profile
-
-`ktrl -init [-global|mongodb] profile_name`
-
-locations for profiles
-
-- mongodb: stored in MongoDB
-- global: `$HOME/kuki/_profile`
-- local: `$PWD/profile`
-
-#### Start Process Using ktrl Profile
-
-`ktrl -profile [-global|mongodb] profile_name`
-
-- with `-mongodb`, ktrl will use profiles in MongoDB
-- with `-global`, ktrl will use profiles in global profile directory
-- without `-global|mongodb`, ktrl will use profiles as following priorities:
-  - local directory
-  - global profile directory
-  - MongoDB
-
-#### Config ktrl
-
-`ktrl -config`
-
-Config ktrl includes MongoDB connection details, configuration file path `$HOME/kuki/_config/ktrlrc.json`
+`kuki` can publish and install packages from central registry site [kuki.ninja](https://kuki.ninja/), thanks to [verdaccio](https://verdaccio.org/)
 
                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `kuki-0.3.0/kuki.egg-info/SOURCES.txt` & `kuki-0.9.7/kuki.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 README.md
 setup.cfg
 setup.py
 kuki/__init__.py
 kuki/config_util.py
 kuki/kest.py
 kuki/ktrl.py
+kuki/ktrl_util.py
 kuki/kuki.py
 kuki/package_util.py
-kuki/profile_util.py
 kuki/registry_util.py
 kuki/util.py
-kuki/version.py
 kuki.egg-info/PKG-INFO
 kuki.egg-info/SOURCES.txt
 kuki.egg-info/dependency_links.txt
 kuki.egg-info/entry_points.txt
 kuki.egg-info/not-zip-safe
 kuki.egg-info/requires.txt
 kuki.egg-info/top_level.txt
```

### Comparing `kuki-0.3.0/test/test_kest.py` & `kuki-0.9.7/test/test_kest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 
-from kuki.util import generate_options
+from kuki.util import generate_process_options
 
 logger = logging.getLogger(__name__)
 
 
 def test_load_kest_json():
     kest_json = {
         "console_size": [50, 160],
@@ -50,15 +50,15 @@
         "1",
         "-r",
         ":localhost:1800",
         "-E",
         "1",
         "-b",
     ]
-    assert generate_options([], kest_json) == expect_args
+    assert generate_process_options([], kest_json) == expect_args
 
 
 def test_skip_args():
     kest_json = {
         "console_size": [50, 160],
         "error_traps": "suspend",
         "garbage_collection": "immediate",
@@ -67,8 +67,8 @@
 
     expect_args = [
         "-e",
         "1",
         "-g",
         "1",
     ]
-    assert generate_options(args, kest_json) == expect_args
+    assert generate_process_options(args, kest_json) == expect_args
```

### Comparing `kuki-0.3.0/test/test_kuki.py` & `kuki-0.9.7/test/test_kuki.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     config_util.global_config_dir = Path.joinpath(config_util.global_kuki_root, "config")
 
     config_util.global_config_dir.mkdir(parents=True, exist_ok=True)
     config_util.global_config_path = Path.joinpath(
         config_util.global_config_dir, config_util.config_file
     )
 
-    global_cache_path = Path.joinpath(global_kuki_root, ".cache")
+    global_cache_path = Path.joinpath(global_kuki_root, "_cache")
     global_cache_path.mkdir(parents=True, exist_ok=True)
     registry_util.global_cache_dir = global_cache_path
 
     global_index_path = Path.joinpath(global_kuki_root, ".index")
     registry_util.global_index_path = global_index_path
 
     dummy_package = Path.joinpath(dir, "dummy")
@@ -89,16 +89,18 @@
 def test_adduser(monkeypatch: pytest.MonkeyPatch):
     responses.add(
         responses.PUT,
         registry_util.user_url + "test",
         json={"token": "7IForS1HdYwD7wgFxXGMTA=="},
         status=201,
     )
-    inputs = iter(["test", "password", "test@test.com"])
+    inputs = iter(["test", "test@test.com", "yes"])
+    password_inputs = iter(["password", "password"])
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
+    monkeypatch.setattr("getpass.getpass", lambda _: next(password_inputs))
     run_kuki("--adduser")
     assert config_util.load_config()["token"] == "7IForS1HdYwD7wgFxXGMTA=="
 
 
 @pytest.mark.parametrize(
     "command_params, expected_token, expected_registry",
     [
@@ -117,14 +119,15 @@
 def test_init(monkeypatch: pytest.MonkeyPatch):
     inputs = iter(
         [
             "dummy",
             "a dummy package",
             "Saitama",
             "https://github.com/saitama/dummy",
+            "q",
             "yes",
         ]
     )
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
     run_kuki("--init")
     kuki_json = package_util.load_kuki()
 
@@ -159,21 +162,18 @@
 def test_login(monkeypatch: pytest.MonkeyPatch):
     responses.add(
         responses.PUT,
         registry_util.user_url + "test",
         json={"token": "7IForS1HdYwD7wgFxXGMTA=="},
         status=201,
     )
-    inputs = iter(
-        [
-            "test",
-            "password",
-        ]
-    )
+    inputs = iter(["test"])
+    password_inputs = iter(["password"])
     monkeypatch.setattr("builtins.input", lambda _: next(inputs))
+    monkeypatch.setattr("getpass.getpass", lambda _: next(password_inputs))
     run_kuki("--login")
     assert config_util.load_config()["token"] == "7IForS1HdYwD7wgFxXGMTA=="
 
 
 @responses.activate
 def test_search():
     search_result = {
@@ -186,15 +186,15 @@
                     "author": {"name": "Saitama"},
                     "repository": {
                         "type": "git",
                         "url": "git+https://github.com/saitama/dummy",
                     },
                     "readmeFilename": "README.md",
                     "homepage": "https://github.com/saitama/dummy#readme",
-                    "keywords": ["q", "kx", "kdb+"],
+                    "keywords": ["q", "k"],
                     "time": {"modified": "2023-04-23T11:36:41.844Z"},
                     "license": "Apache-2.0",
                     "versions": {"1.1.5": "latest"},
                 },
             }
         ],
         "total": 1,
@@ -406,14 +406,54 @@
     dependencies = package_util.load_kuki()["dependencies"]
     assert len(dependencies) == len(expected_deps)
     for dep in expected_deps:
         assert dep in dependencies
 
 
 @pytest.mark.parametrize(
+    "command_params, expected_index",
+    [
+        ("--global --install log", ["log@0.1.1"]),
+        ("--global --install file", ["file@1.0.1", "log@0.1.1"]),
+        (
+            "--global --install csv",
+            ["csv@0.0.2", "file@1.0.0", "log@0.1.0"],
+        ),
+        (
+            "--global --install csv@0.0.1",
+            ["csv@0.0.1", "file@1.0.0", "log@0.1.0"],
+        ),
+        (
+            "--global --install file log",
+            ["file@1.0.1", "log@0.1.1"],
+        ),
+        (
+            "--global --install file log@0.1.0",
+            ["file@1.0.1", "log@0.1.1", "log@0.1.0"],
+        ),
+    ],
+)
+@responses.activate
+def test_install_in_global_mode(
+    mock_package_api,
+    command_params,
+    expected_index: List[str],
+):
+    run_kuki(command_params)
+    global_index = registry_util.load_global_index()
+    assert len(global_index) == len(expected_index)
+
+    for pkg_id in expected_index:
+        assert pkg_id in global_index
+        name, version = pkg_id.split("@")
+        pkg_dir = Path.joinpath(config_util.global_kuki_root, name, version)
+        assert Path.joinpath(pkg_dir, package_util.config_file).exists()
+
+
+@pytest.mark.parametrize(
     "command_params, expected_index, expected_pkg_index, expected_deps",
     [
         (
             "--uninstall csv",
             ["csv@0.0.2", "file@1.0.1", "file@1.0.0", "log@0.1.1", "log@0.1.0"],
             ["file", "log"],
             ["file"],
```

