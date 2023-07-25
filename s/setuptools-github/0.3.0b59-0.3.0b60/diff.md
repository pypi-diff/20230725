# Comparing `tmp/setuptools-github-0.3.0b59.tar.gz` & `tmp/setuptools-github-0.3.0b60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setuptools-github-0.3.0b59.tar", last modified: Mon Jul 24 16:54:02 2023, max compression
+gzip compressed data, was "setuptools-github-0.3.0b60.tar", last modified: Tue Jul 25 14:17:49 2023, max compression
```

## Comparing `setuptools-github-0.3.0b59.tar` & `setuptools-github-0.3.0b60.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/setuptools_github.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8887 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/setuptools_github.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.987473 setuptools-github-0.3.0b59/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/src/setuptools_github/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-24 16:54:02.000000 setuptools-github-0.3.0b59/src/setuptools_github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/src/setuptools_github/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 16:54:02.991473 setuptools-github-0.3.0b59/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-24 16:53:35.000000 setuptools-github-0.3.0b59/tests/test_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.608185 setuptools-github-0.3.0b60/setuptools_github.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/setuptools_github.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.604185 setuptools-github-0.3.0b60/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.608185 setuptools-github-0.3.0b60/src/setuptools_github/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-25 14:17:49.000000 setuptools-github-0.3.0b60/src/setuptools_github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4947 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/src/setuptools_github/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:17:49.612185 setuptools-github-0.3.0b60/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-07-25 14:17:18.000000 setuptools-github-0.3.0b60/tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b59/LICENSE` & `setuptools-github-0.3.0b60/LICENSE`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/setup.py` & `setuptools-github-0.3.0b60/setup.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/setuptools_github.egg-info/SOURCES.txt` & `setuptools-github-0.3.0b60/setuptools_github.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,8 +17,9 @@
 src/setuptools_github/tools.py
 tests/conftest.py
 tests/requirements.txt
 tests/test_checks.py
 tests/test_cli.py
 tests/test_conftest.py
 tests/test_scm.py
+tests/test_script.py
 tests/test_tools.py
```

### Comparing `setuptools-github-0.3.0b59/src/setuptools_github/checks.py` & `setuptools-github-0.3.0b60/src/setuptools_github/checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/src/setuptools_github/cli.py` & `setuptools-github-0.3.0b60/src/setuptools_github/cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/src/setuptools_github/tools.py` & `setuptools-github-0.3.0b60/src/setuptools_github/tools.py`

 * *Files 3% similar despite different names*

```diff
@@ -254,14 +254,16 @@
 
     version = current = get_module_var(path, "__version__")
 
     expr = re.compile(r"/(?P<what>beta|release)/(?P<version>\d+([.]\d+)*)$")
     expr1 = re.compile(r"(?P<version>\d+([.]\d+)*)(?P<num>b\d+)?$")
 
     if match := expr.search(gdata["ref"]):
+        # setuptools double calls the update_version,
+        # this fixes the issue
         match1 = expr1.search(current or "")
         if not match1:
             raise InvalidGithubReference(f"cannot parse current version '{current}'")
         if match1.group("version") != match.group("version"):
             raise InvalidGithubReference(
                 f"building package for {current} from '{gdata['ref']}' "
                 f"branch ({match.groupdict()} mismatch {match1.groupdict()})"
```

### Comparing `setuptools-github-0.3.0b59/tests/test_checks.py` & `setuptools-github-0.3.0b60/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/tests/test_cli.py` & `setuptools-github-0.3.0b60/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/tests/test_conftest.py` & `setuptools-github-0.3.0b60/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `setuptools-github-0.3.0b59/tests/test_tools.py` & `setuptools-github-0.3.0b60/tests/test_tools.py`

 * *Files identical despite different names*

