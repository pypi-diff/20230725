# Comparing `tmp/keyring_pybridge-0.3.0.tar.gz` & `tmp/keyring_pybridge-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keyring_pybridge-0.3.0.tar", max compression
+gzip compressed data, was "keyring_pybridge-0.4.0.tar", max compression
```

## Comparing `keyring_pybridge-0.3.0.tar` & `keyring_pybridge-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1459 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/README.md
--rw-r--r--   0        0        0       68 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/keyring_pybridge/__init__.py
--rw-r--r--   0        0        0     2127 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/keyring_pybridge/backend.py
--rw-r--r--   0        0        0      729 2023-07-24 13:35:26.115597 keyring_pybridge-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1977 1970-01-01 00:00:00.000000 keyring_pybridge-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1459 2023-07-25 13:08:13.795989 keyring_pybridge-0.4.0/README.md
+-rw-r--r--   0        0        0       74 2023-07-25 13:08:13.795989 keyring_pybridge-0.4.0/keyring_pybridge/__init__.py
+-rw-r--r--   0        0        0     2651 2023-07-25 13:08:13.795989 keyring_pybridge-0.4.0/keyring_pybridge/backend.py
+-rw-r--r--   0        0        0      730 2023-07-25 13:08:13.795989 keyring_pybridge-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1972 1970-01-01 00:00:00.000000 keyring_pybridge-0.4.0/PKG-INFO
```

### Comparing `keyring_pybridge-0.3.0/README.md` & `keyring_pybridge-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `keyring_pybridge-0.3.0/keyring_pybridge/backend.py` & `keyring_pybridge-0.4.0/keyring_pybridge/backend.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 from functools import cache
 import json
 from pathlib import Path
 from shutil import which
-from subprocess import run
+from subprocess import CalledProcessError, run
 from sys import executable
 
 from keyring.backend import KeyringBackend
+from keyring.errors import *  # noqa: F403
 
 
-def call_python_keyring(python, command):
-    p = run(
-        [python, "-c", f"import keyring; {command}"], shell=False, capture_output=True
-    )
-    stdout, stderr = p.stdout.decode("utf-8").strip(), p.stderr.decode("utf-8").strip()
-    if p.returncode != 0:
-        raise RuntimeError(
-            f"call to WSL host keyring failed (python path: {python}): {stderr}"
-        )
-    return stdout
+def run_command(command, encoding="utf-8"):
+    p = run(command, shell=False, capture_output=True, check=True)
+    return p.stdout.decode(encoding).strip()
 
 
 @cache
 def check_python(python):
     if not python:
         raise ValueError("please configure KEYRING_PROPERTY_PYTHON")
     py_self = Path(executable).resolve()
@@ -31,41 +25,71 @@
     if not py_bridge.is_file():
         raise ValueError(f"{python} is not a file")
     if py_self == py_bridge:
         raise ValueError(
             "please configure KEYRING_PROPERTY_PYTHON to a python"
             f" executable other than {executable}"
         )
-    call_python_keyring(python, "")
+    run_command([python, "-c", "print('check')"])
+
+
+@cache
+def get_encoding(python):
+    return run_command([python, "-c", "import sys; print(sys.stdout.encoding)"])
+
+
+def call_keyring(python, command):
+    check_python(python)
+    encoding = get_encoding(python)
+    code = """import keyring
+import sys
+try:
+    {command}
+except keyring.errors.KeyringError as err:
+    print(repr(err), file=sys.stderr)
+    sys.exit(100)
+""".format(
+        command=command
+    )
+    try:
+        return run_command([python, "-c", code], encoding=encoding)
+    except CalledProcessError as err:
+        if err.returncode == 100:
+            stderr = err.stderr.decode(encoding).strip()
+            exc = eval(stderr)
+            raise exc
+        else:
+            raise
 
 
 def format_args(*args):
     return ", ".join(map(repr, args))
 
 
 class PyBridgeKeyring(KeyringBackend):
     priority = 1
     python = ""
 
     def set_password(self, servicename, username, password):
-        check_python(self.python)
-        call_python_keyring(
+        call_keyring(
             self.python,
             f"keyring.set_password({format_args(servicename, username, password)})",
         )
 
     def get_password(self, servicename, username):
-        check_python(self.python)
         args = format_args(servicename, username)
         return json.loads(
-            call_python_keyring(
+            call_keyring(
                 self.python,
-                f"import json; print(json.dumps(keyring.get_password({args})))",
+                (
+                    f"import json; print("
+                    f"json.dumps(keyring.get_password({args}), ensure_ascii=False)"
+                    f")"
+                ),
             )
         )
 
     def delete_password(self, servicename, username):
-        check_python(self.python)
-        call_python_keyring(
+        call_keyring(
             self.python,
             f"keyring.delete_password({format_args(servicename, username)})",
         )
```

### Comparing `keyring_pybridge-0.3.0/pyproject.toml` & `keyring_pybridge-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "keyring-pybridge"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Korijn van Golen <korijn.vangolen@zimmerbiomet.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
-keyring = "~24.2.0"
+python = ">=3.9"
+keyring = "^24.2.0"
 
 [tool.poetry.group.dev.dependencies]
-ruff = "~0.0.278"
-black = "~23.7.0"
-twine = "~4.0.2"
-pytest = "~7.4.0"
+ruff = "^0.0.278"
+black = "^23.7.0"
+twine = "^4.0.2"
+pytest = "^7.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 select = [
```

### Comparing `keyring_pybridge-0.3.0/PKG-INFO` & `keyring_pybridge-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: keyring-pybridge
-Version: 0.3.0
+Version: 0.4.0
 Summary: 
 License: MIT
 Author: Korijn van Golen
 Author-email: korijn.vangolen@zimmerbiomet.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: keyring (>=24.2.0,<24.3.0)
+Requires-Dist: keyring (>=24.2.0,<25.0.0)
 Description-Content-Type: text/markdown
 
 # keyring-pybridge
 
 [![CI](https://github.com/clinicalgraphics/keyring-pybridge/actions/workflows/ci.yml/badge.svg)](https://github.com/clinicalgraphics/keyring-pybridge/actions/workflows/ci.yml)
 [![PyPI version ](https://badge.fury.io/py/keyring-pybridge.svg)
 ](https://badge.fury.io/py/keyring-pybridge)
```

