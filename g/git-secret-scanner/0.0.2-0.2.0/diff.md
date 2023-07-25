# Comparing `tmp/git_secret_scanner-0.0.2.tar.gz` & `tmp/git_secret_scanner-0.2.0.tar.gz`

## Comparing `git_secret_scanner-0.0.2.tar` & `git_secret_scanner-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/pyrightconfig.json
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/renovate.json
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/requirements.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/ruff.toml
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/__main__.py
--rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/cli.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/git.py
--rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/scan.py
--rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/scanners.py
--rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/src/git_secret_scanner/secret.py
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/LICENSE
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/README.md
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/hatch.toml
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 git_secret_scanner-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/pyrightconfig.json
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/renovate.json
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/requirements.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/ruff.toml
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/__main__.py
+-rwxr-xr-x   0        0        0     2583 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/cli.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/git.py
+-rw-r--r--   0        0        0     4540 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/scan.py
+-rw-r--r--   0        0        0     3764 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/scanners.py
+-rw-r--r--   0        0        0     2075 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/src/git_secret_scanner/secret.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/README.md
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/hatch.toml
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4637 2020-02-02 00:00:00.000000 git_secret_scanner-0.2.0/PKG-INFO
```

### Comparing `git_secret_scanner-0.0.2/src/git_secret_scanner/cli.py` & `git_secret_scanner-0.2.0/src/git_secret_scanner/cli.py`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/src/git_secret_scanner/git.py` & `git_secret_scanner-0.2.0/src/git_secret_scanner/git.py`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/src/git_secret_scanner/scan.py` & `git_secret_scanner-0.2.0/src/git_secret_scanner/scan.py`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/src/git_secret_scanner/scanners.py` & `git_secret_scanner-0.2.0/src/git_secret_scanner/scanners.py`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/src/git_secret_scanner/secret.py` & `git_secret_scanner-0.2.0/src/git_secret_scanner/secret.py`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/LICENSE` & `git_secret_scanner-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/README.md` & `git_secret_scanner-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/pyproject.toml` & `git_secret_scanner-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `git_secret_scanner-0.0.2/PKG-INFO` & `git_secret_scanner-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-secret-scanner
-Version: 0.0.2
+Version: 0.2.0
 Summary: Find secrets in git repositories with TruffleHog & Gitleaks
 Project-URL: Homepage, https://github.com/padok-team/git-secret-scanner
 Project-URL: Repository, https://github.com/padok-team/git-secret-scanner
 Author: Padok
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: git,scan,secret,security
```

