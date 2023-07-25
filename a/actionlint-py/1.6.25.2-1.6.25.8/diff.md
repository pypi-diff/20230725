# Comparing `tmp/actionlint_py-1.6.25.2.tar.gz` & `tmp/actionlint_py-1.6.25.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "actionlint_py-1.6.25.2.tar", last modified: Sun Jul  9 19:21:18 2023, max compression
+gzip compressed data, was "actionlint_py-1.6.25.8.tar", last modified: Tue Jul 25 08:29:06 2023, max compression
```

## Comparing `actionlint_py-1.6.25.2.tar` & `actionlint_py-1.6.25.8.tar`

### file list

```diff
@@ -1,11 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 19:21:18.577056 actionlint_py-1.6.25.2/
--rw-rw-rw-   0        0        0     1087 2023-05-03 15:51:52.000000 actionlint_py-1.6.25.2/LICENSE
--rw-rw-rw-   0        0        0     2081 2023-07-09 19:21:18.577056 actionlint_py-1.6.25.2/PKG-INFO
--rw-rw-rw-   0        0        0     1380 2023-07-09 19:19:45.000000 actionlint_py-1.6.25.2/README.md
-drwxrwxrwx   0        0        0        0 2023-07-09 19:21:18.576054 actionlint_py-1.6.25.2/actionlint_py.egg-info/
--rw-rw-rw-   0        0        0     2081 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      184 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-09 19:21:18.000000 actionlint_py-1.6.25.2/actionlint_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1737 2023-07-09 19:21:18.578389 actionlint_py-1.6.25.2/setup.cfg
--rw-rw-rw-   0        0        0     5099 2023-05-03 17:13:49.000000 actionlint_py-1.6.25.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_ACTIONLINT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_BUILD_SYSTEM.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/VERSION_DEV.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/auto_update_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/checksums.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/bdist_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/fetch_binaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/commands/install_actionlint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/_custom_build/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/utils/file_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/_custom_build/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/actionlint_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4231 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-25 08:29:06.000000 actionlint_py-1.6.25.8/actionlint_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-07-25 08:28:46.000000 actionlint_py-1.6.25.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:29:06.270712 actionlint_py-1.6.25.8/setup.cfg
```

### Comparing `actionlint_py-1.6.25.2/PKG-INFO` & `actionlint_py-1.6.25.8/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,72 +1,71 @@
-Metadata-Version: 2.1
-Name: actionlint_py
-Version: 1.6.25.2
-Summary: Python wrapper around invoking actionlint (https://github.com/rhysd/actionlint)
-Home-page: https://github.com/Mateusz-Grzelinski/actionlint-py
-Author: Ryan Rhee, Mateusz Grzeliński
-Author-email: grzelinskimat@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# actionlint-py
-
-A python wrapper to provide a pip-installable [actionlint] binary.
-
-Internally this package provides a convenient way to download the pre-built
-actionlint binary for your particular platform.
-
-### Installation
-
-```bash
-pip install actionlint-py
-```
-
-### Usage
-
-After installation, the `actionlint` binary should be available in your
-environment (or `actionlint.exe` on windows).
-
-### As a pre-commit hook
-
-See [pre-commit] for instructions
-
-Sample `.pre-commit-config.yaml`:
-
-```yaml
-- repo: https://github.com/Mateusz-Grzelinski/actionlint-py
-  rev: v1.6.25
-  hooks:
-    - id: actionlint
-```
-
-or to avoid going twice to internet (might help with proxy):
-
-```yaml
-- repo: local
-  hooks:
-    - id: actionlint
-      name: actionlint
-      description: Test yaml scripts with actionlint
-      #      additional_dependencies: [actionlint-py==1.6.22.2] # safer, but pre-commit autoupdate will not work
-      additional_dependencies: [ actionlint-py ]
-      entry: actionlint
-      #      args: [-ignore "*.set-output. was depracated.*"]
-      language: python
-      types: [ "yaml" ]
-      files: "^.github/workflows/"
-```
-
-[actionlint]: https://github.com/rhysd/actionlint
-
-[pre-commit]: https://pre-commit.com
-
-# Development
-
-Development of wrapper and releasing new version: see [README-DEV.md](README-DEV.md)
+# actionlint-py
+
+A python wrapper to provide a pip-installable [actionlint] binary.
+
+Internally this package provides a convenient way to download the pre-built
+actionlint binary for your particular platform.
+
+### Installation
+
+```bash
+pip install actionlint-py
+```
+
+### Usage
+
+After installation, the `actionlint` binary should be available in your
+environment (or `actionlint.exe` on windows).
+
+### As a pre-commit hook
+
+See [pre-commit] for instructions
+
+Sample `.pre-commit-config.yaml`:
+
+```yaml
+- repo: https://github.com/Mateusz-Grzelinski/actionlint-py
+  rev: v1.6.25.5
+  hooks:
+    - id: actionlint
+```
+
+Because `actionlint-py` is available as source distribution, pip build system is set up to fetch binary from (public)
+github. It might cause problems with corporate proxy. In case of problems try this semi-manual setup:
+
+```yaml
+- repo: local
+  hooks:
+    - id: actionlint
+      name: actionlint
+      description: Lint GitHub workflows with actionlint
+      additional_dependencies: [ actionlint-py ]
+      #additional_dependencies: [actionlint-py==1.6.25.5]
+      # safer, but pre-commit autoupdate will not work
+      # note: the versioning scheme is different: not "v1.6.25" but "1.6.25.2" (last number is build system version)
+      entry: actionlint
+      #args: [-ignore "*.set-output. was depracated.*"]
+      language: python
+      types: [ "yaml" ]
+      files: "^.github/workflows/"
+```
+
+[actionlint]: https://github.com/rhysd/actionlint
+
+[pre-commit]: https://pre-commit.com
+
+# Development
+
+Development of wrapper and releasing new version:
+see [README-DEV.md](https://github.com/Mateusz-Grzelinski/actionlint-py/blob/main/README-DEV.md)
+
+# Roadmap
+
+- [ ] Update tag in readme in github action when releasing new version
+- [ ] Upload also binary distribution, not only source distribution
+- [ ] Add unit tests to build system
+
+See [README-DEV.md](https://github.com/Mateusz-Grzelinski/actionlint-py/blob/main/README-DEV.md) for more TODOs.
+
+Won't do unless asked:
+
+- support all platforms that actionlint supports (like freebsd)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

