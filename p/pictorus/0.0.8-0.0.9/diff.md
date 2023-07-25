# Comparing `tmp/pictorus-0.0.8.tar.gz` & `tmp/pictorus-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pictorus-0.0.8.tar", last modified: Wed Jun 21 04:43:14 2023, max compression
+gzip compressed data, was "pictorus-0.0.9.tar", last modified: Tue Jul 25 03:05:42 2023, max compression
```

## Comparing `pictorus-0.0.8.tar` & `pictorus-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      710 2023-06-21 04:42:19.636723 pictorus-0.0.8/.github/workflows/test.yaml
--rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.8/.gitignore
--rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.0.8/.python-version
--rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.8/LICENSE
--rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.0.8/PUB_README.md
--rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.8/README.md
--rw-r--r--   0        0        0      829 2023-06-21 04:42:19.637210 pictorus-0.0.8/pyproject.toml
--rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.8/script/setup
--rw-r--r--   0        0        0       61 2023-06-21 04:42:39.631742 pictorus-0.0.8/src/pictorus/__init__.py
--rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.8/src/pictorus/app_manager.py
--rw-r--r--   0        0        0     3297 2023-06-21 04:42:19.637658 pictorus-0.0.8/src/pictorus/config.py
--rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.8/src/pictorus/constants.py
--rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.8/src/pictorus/logging.py
--rw-r--r--   0        0        0     5041 2023-06-21 04:42:19.638038 pictorus-0.0.8/src/pictorus/pictorus_cli.py
--rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.8/src/pictorus/pictorus_device_manager.py
--rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.8/src/pictorus/systemd.py
--rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.8/src/pictorus/telemetry_manager.py
--rw-r--r--   0        0        0     3328 2023-06-21 04:42:19.638345 pictorus-0.0.8/src/pictorus/version_manager.py
--rw-r--r--   0        0        0     8967 2023-06-21 04:42:19.638752 pictorus-0.0.8/tests/pictorus/test_app_manager.py
--rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.0.8/tests/pictorus/test_version_manager.py
--rw-r--r--   0        0        0     1358 1970-01-01 00:00:00.000000 pictorus-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      710 2023-06-21 04:42:19.636723 pictorus-0.0.9/.github/workflows/test.yaml
+-rw-r--r--   0        0        0      918 2023-02-14 23:52:57.501277 pictorus-0.0.9/.gitignore
+-rw-r--r--   0        0        0        6 2023-06-20 17:57:52.943257 pictorus-0.0.9/.python-version
+-rw-r--r--   0        0        0    32422 2023-02-15 19:48:07.053335 pictorus-0.0.9/LICENSE
+-rw-r--r--   0        0        0      749 2023-06-19 23:08:46.580929 pictorus-0.0.9/PUB_README.md
+-rw-r--r--   0        0        0     1433 2023-03-30 22:18:14.564827 pictorus-0.0.9/README.md
+-rw-r--r--   0        0        0      909 2023-07-11 00:18:37.316414 pictorus-0.0.9/pyproject.toml
+-rwxr-xr-x   0        0        0      340 2023-02-15 19:48:07.054532 pictorus-0.0.9/script/setup
+-rw-r--r--   0        0        0       61 2023-07-25 03:05:21.292582 pictorus-0.0.9/src/pictorus/__init__.py
+-rw-r--r--   0        0        0    14247 2023-05-19 20:28:20.661444 pictorus-0.0.9/src/pictorus/app_manager.py
+-rw-r--r--   0        0        0     3297 2023-06-21 04:42:19.637658 pictorus-0.0.9/src/pictorus/config.py
+-rw-r--r--   0        0        0      492 2023-05-09 19:07:56.162364 pictorus-0.0.9/src/pictorus/constants.py
+-rw-r--r--   0        0        0      244 2023-02-15 19:48:07.055277 pictorus-0.0.9/src/pictorus/logging.py
+-rw-r--r--   0        0        0     5647 2023-07-25 03:04:55.014509 pictorus-0.0.9/src/pictorus/pictorus_cli.py
+-rwxr-xr-x   0        0        0     2390 2023-05-19 20:28:20.663228 pictorus-0.0.9/src/pictorus/pictorus_device_manager.py
+-rw-r--r--   0        0        0     1476 2023-02-16 17:48:01.978870 pictorus-0.0.9/src/pictorus/systemd.py
+-rw-r--r--   0        0        0     4878 2023-05-09 19:07:56.163315 pictorus-0.0.9/src/pictorus/telemetry_manager.py
+-rw-r--r--   0        0        0     3328 2023-06-21 04:42:19.638345 pictorus-0.0.9/src/pictorus/version_manager.py
+-rw-r--r--   0        0        0     8967 2023-06-21 04:42:19.638752 pictorus-0.0.9/tests/pictorus/test_app_manager.py
+-rw-r--r--   0        0        0     2532 2023-06-21 04:42:19.639081 pictorus-0.0.9/tests/pictorus/test_version_manager.py
+-rw-r--r--   0        0        0     1439 1970-01-01 00:00:00.000000 pictorus-0.0.9/PKG-INFO
```

### Comparing `pictorus-0.0.8/.github/workflows/test.yaml` & `pictorus-0.0.9/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/.gitignore` & `pictorus-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/LICENSE` & `pictorus-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/PUB_README.md` & `pictorus-0.0.9/PUB_README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/README.md` & `pictorus-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/pyproject.toml` & `pictorus-0.0.9/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 name = "pictorus"
 authors = [{ name = "Pictorus Inc", email = "contact@pictor.us" }]
 license = { file = "LICENSE" }
 classifiers = [
   "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
 dynamic = ["version", "description"]
-dependencies = ["awsiotsdk~=1.11.5", "requests~=2.26.0", "semver~=2.13.0"]
+dependencies = [
+  "awsiotsdk~=1.11.5",
+  'requests~=2.27.1; python_version <= "3.6"',
+  'requests~=2.31.0; python_version > "3.6"',
+  "semver~=2.13.0",
+]
 requires-python = ">=3.6"
 readme = "PUB_README.md"
 
 [project.scripts]
 pictorus-cli = "pictorus.pictorus_cli:main"
 pictorus-device-manager = "pictorus.pictorus_device_manager:main"
```

### Comparing `pictorus-0.0.8/src/pictorus/app_manager.py` & `pictorus-0.0.9/src/pictorus/app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/src/pictorus/config.py` & `pictorus-0.0.9/src/pictorus/config.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/src/pictorus/pictorus_cli.py` & `pictorus-0.0.9/src/pictorus/pictorus_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,17 +60,17 @@
 
 
 def configure_additional_settings():
     """Configure any additional settings that require user input"""
     config.auto_update = prompt_auto_update()
 
 
-def configure():
+def configure(args: argparse.Namespace):
     """Configure the device manager"""
-    configure_device()
+    configure_device(token=args.token)
     setup_device_manager()
     configure_additional_settings()
 
 
 def setup_device_manager():
     """Setup and start the device manager service"""
     print("Setting up device manager service")
@@ -96,26 +96,32 @@
         "Service to manage Pictorus apps",
         bin_path,
     )
     printf("Configured device manager service", TextFormat.OKGREEN)
 
 
 def try_device_configuration(
-    device_name: str, system_data: dict, credentials: Tuple[str, str]
+    device_name: str, system_data: dict, credentials: Tuple[str, str] = None, token: str = None
 ) -> bool:
     """Try to configure the device"""
-    session = requests.Session()
-    session.auth = credentials
+    if not credentials and not token:
+        raise ValueError("Either user/pass credentials or token must be provided")
 
-    res = session.post(
+    headers = {}
+    if token:
+        headers["Authorization"] = f"Bearer {token}"
+
+    res = requests.post(
         urljoin(API_PREFIX, "v2/devices"),
         json={
             "name": device_name,
             "system": system_data,
         },
+        headers=headers,
+        auth=credentials,
     )
 
     if not res.ok:
         try:
             message = res.json().get("message", DEFAULT_AUTH_ERROR)
         except json.JSONDecodeError:
             message = DEFAULT_AUTH_ERROR
@@ -123,15 +129,15 @@
         printf(f"Failed to configure device: {message}", TextFormat.FAIL)
         return False
 
     config.store_config(res.json())
     return True
 
 
-def configure_device():
+def configure_device(token: str = None):
     """Configure this device to connect to pictorus"""
     print("Configuring new device")
     if not config.is_empty():
         confirm = input(
             "It looks like this device is already configured. Would you like to overwrite it [y/N]? "
         )
         if confirm.lower() != "y":
@@ -144,37 +150,45 @@
 
     system_data = {
         "platform": platform.platform(),
         "system": platform.system(),
         "machine": platform.machine(),
     }
 
-    configured = False
-    username = None
-    while not configured:
-        credentials = get_credentials(username)
-        # Cache the username so user doesn't have to input again on failure
-        username = credentials[0]
-        configured = try_device_configuration(device_name, system_data, credentials)
+    if token:
+        if not try_device_configuration(device_name, system_data, token=token):
+            raise SystemExit(1)
+    else:
+        configured = False
+        username = None
+        while not configured:
+            credentials = get_credentials(username)
+            # Cache the username so user doesn't have to input again on failure
+            username = credentials[0]
+            configured = try_device_configuration(device_name, system_data, credentials=credentials)
 
     printf(f"Successfully configured device: {device_name}", TextFormat.OKGREEN)
 
 
 def main():
     """Main CLI entry point"""
     parser = argparse.ArgumentParser(description="Pictorus device manager")
     subparsers = parser.add_subparsers()
 
     parser_config = subparsers.add_parser("configure", help="Configure this device")
+    parser_config.add_argument(
+        "--token",
+        help="Authentication token. If not provided, you will be prompted for credentials",
+    )
     parser_config.set_defaults(func=configure)
 
     args = parser.parse_args()
 
     if not hasattr(args, "func"):
         parser.print_help()
         sys.exit(0)
 
-    args.func()
+    args.func(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pictorus-0.0.8/src/pictorus/pictorus_device_manager.py` & `pictorus-0.0.9/src/pictorus/pictorus_device_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/src/pictorus/systemd.py` & `pictorus-0.0.9/src/pictorus/systemd.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/src/pictorus/telemetry_manager.py` & `pictorus-0.0.9/src/pictorus/telemetry_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/src/pictorus/version_manager.py` & `pictorus-0.0.9/src/pictorus/version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/tests/pictorus/test_app_manager.py` & `pictorus-0.0.9/tests/pictorus/test_app_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/tests/pictorus/test_version_manager.py` & `pictorus-0.0.9/tests/pictorus/test_version_manager.py`

 * *Files identical despite different names*

### Comparing `pictorus-0.0.8/PKG-INFO` & `pictorus-0.0.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: pictorus
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pictorus device manager package
 Author-email: Pictorus Inc <contact@pictor.us>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: awsiotsdk~=1.11.5
-Requires-Dist: requests~=2.26.0
+Requires-Dist: requests~=2.27.1; python_version <= "3.6"
+Requires-Dist: requests~=2.31.0; python_version > "3.6"
 Requires-Dist: semver~=2.13.0
 Requires-Dist: black==22.3.0 ; extra == "dev"
 Requires-Dist: responses==0.17.0 ; extra == "test"
 Requires-Dist: pytest==7.0.1 ; extra == "test"
 Project-URL: Home, https://pictor.us
 Provides-Extra: dev
 Provides-Extra: test
```

