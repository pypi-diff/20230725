# Comparing `tmp/redsession-1.0.1.tar.gz` & `tmp/redsession-1.0.2.tar.gz`

## Comparing `redsession-1.0.1.tar` & `redsession-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.0.1/.readthedocs.yaml
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.0.1/requirements-docs.txt
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.0.1/requirements-tests.txt
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.0.1/requirements.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 redsession-1.0.1/redsession/__init__.py
--rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 redsession-1.0.1/redsession/middleware.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 redsession-1.0.1/redsession/backend/__init__.py
--rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.0.1/redsession/backend/base.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 redsession-1.0.1/redsession/backend/redis.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.0.1/tests/__init__.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 redsession-1.0.1/tests/test_session.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.0.1/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.0.1/LICENSE.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.0.1/README.rst
--rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 redsession-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 redsession-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 redsession-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 redsession-1.0.2/.readthedocs.yaml
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements-docs.txt
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements-tests.txt
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 redsession-1.0.2/requirements.txt
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/__init__.py
+-rw-r--r--   0        0        0     5964 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/middleware.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/__init__.py
+-rw-r--r--   0        0        0     2080 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/base.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 redsession-1.0.2/redsession/backend/redis.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 redsession-1.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 redsession-1.0.2/tests/test_session.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 redsession-1.0.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 redsession-1.0.2/LICENSE.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 redsession-1.0.2/README.rst
+-rw-r--r--   0        0        0     1169 2020-02-02 00:00:00.000000 redsession-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 redsession-1.0.2/PKG-INFO
```

### Comparing `redsession-1.0.1/.pre-commit-config.yaml` & `redsession-1.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/.readthedocs.yaml` & `redsession-1.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/redsession/middleware.py` & `redsession-1.0.2/redsession/middleware.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/redsession/backend/base.py` & `redsession-1.0.2/redsession/backend/base.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/redsession/backend/redis.py` & `redsession-1.0.2/redsession/backend/redis.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/tests/test_session.py` & `redsession-1.0.2/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/LICENSE.md` & `redsession-1.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/README.rst` & `redsession-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/pyproject.toml` & `redsession-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `redsession-1.0.1/PKG-INFO` & `redsession-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redsession
-Version: 1.0.1
+Version: 1.0.2
 Summary: Simple and fastest library for Redis server sessions
 Project-URL: Repository, https://github.com/TheJecksMan/red-session
 Project-URL: Docs, https://red-session.readthedocs.io/en/stable/
 Author: TheJecksMan
 License-Expression: MIT
 License-File: LICENSE.md
 Classifier: Development Status :: 4 - Beta
```

