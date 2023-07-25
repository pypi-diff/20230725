# Comparing `tmp/timedctl-5.0.2.tar.gz` & `tmp/timedctl-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timedctl-5.0.2.tar", max compression
+gzip compressed data, was "timedctl-5.0.3.tar", max compression
```

## Comparing `timedctl-5.0.2.tar` & `timedctl-5.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    34454 2023-07-24 07:10:31.837005 timedctl-5.0.2/LICENSE
--rw-r--r--   0        0        0      774 2023-07-24 07:10:31.837005 timedctl-5.0.2/README.md
--rw-r--r--   0        0        0      849 2023-07-24 07:10:56.961224 timedctl-5.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-24 07:10:31.837005 timedctl-5.0.2/timedctl/__init__.py
--rwxr-xr-x   0        0        0    17405 2023-07-24 07:10:31.837005 timedctl-5.0.2/timedctl/timedctl.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.2/PKG-INFO
+-rw-r--r--   0        0        0    34454 2023-07-25 08:57:31.776332 timedctl-5.0.3/LICENSE
+-rw-r--r--   0        0        0      774 2023-07-25 08:57:31.776332 timedctl-5.0.3/README.md
+-rw-r--r--   0        0        0      849 2023-07-25 08:57:52.532551 timedctl-5.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 08:57:31.780332 timedctl-5.0.3/timedctl/__init__.py
+-rwxr-xr-x   0        0        0    17405 2023-07-25 08:57:31.780332 timedctl-5.0.3/timedctl/timedctl.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 timedctl-5.0.3/PKG-INFO
```

### Comparing `timedctl-5.0.2/LICENSE` & `timedctl-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.2/README.md` & `timedctl-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.2/pyproject.toml` & `timedctl-5.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "timedctl"
-version = "5.0.2"
+version = "5.0.3"
 description = "CLI for timed"
 authors = ["Arthur Deierlein <arthur.deierlein@adfinis.com>", "Gian Klug <gian.klug@adfinis.com>"]
 readme = "README.md"
 license = "AGPL-3.0-only"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 pyfzf = "^0.3.1"
 rich = "^13.4.2"
-libtimed = "^0.4.1"
+libtimed = "^0.4.3"
 terminaltables = "^3.1.10"
 tomlkit = "^0.11.8"
 click-aliases = "^1.0.1"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.3.0"
```

### Comparing `timedctl-5.0.2/timedctl/timedctl.py` & `timedctl-5.0.3/timedctl/timedctl.py`

 * *Files identical despite different names*

### Comparing `timedctl-5.0.2/PKG-INFO` & `timedctl-5.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: timedctl
-Version: 5.0.2
+Version: 5.0.3
 Summary: CLI for timed
 License: AGPL-3.0-only
 Author: Arthur Deierlein
 Author-email: arthur.deierlein@adfinis.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: click-aliases (>=1.0.1,<2.0.0)
-Requires-Dist: libtimed (>=0.4.1,<0.5.0)
+Requires-Dist: libtimed (>=0.4.3,<0.5.0)
 Requires-Dist: pyfzf (>=0.3.1,<0.4.0)
 Requires-Dist: rich (>=13.4.2,<14.0.0)
 Requires-Dist: terminaltables (>=3.1.10,<4.0.0)
 Requires-Dist: tomlkit (>=0.11.8,<0.12.0)
 Description-Content-Type: text/markdown
 
 # timedctl
```

