# Comparing `tmp/swh.journal-1.3.4.tar.gz` & `tmp/swh.journal-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swh.journal-1.3.4.tar", last modified: Thu Jul 13 08:03:33 2023, max compression
+gzip compressed data, was "swh.journal-1.3.5.tar", last modified: Tue Jul 25 08:45:43 2023, max compression
```

## Comparing `swh.journal-1.3.4.tar` & `swh.journal-1.3.5.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-07-13 08:03:27.000000 swh.journal-1.3.4/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-13 08:03:27.000000 swh.journal-1.3.4/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-13 08:03:27.000000 swh.journal-1.3.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-13 08:03:27.000000 swh.journal-1.3.4/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-13 08:03:27.000000 swh.journal-1.3.4/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-07-13 08:03:27.000000 swh.journal-1.3.4/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-13 08:03:27.000000 swh.journal-1.3.4/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-13 08:03:33.392235 swh.journal-1.3.4/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-07-13 08:03:27.000000 swh.journal-1.3.4/README.md
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/example-journal-client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-07-13 08:03:27.000000 swh.journal-1.3.4/docs/journal-clients.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-07-13 08:03:27.000000 swh.journal-1.3.4/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-13 08:03:27.000000 swh.journal-1.3.4/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-07-13 08:03:27.000000 swh.journal-1.3.4/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      405 2023-07-13 08:03:27.000000 swh.journal-1.3.4/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-13 08:03:33.392235 swh.journal-1.3.4/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-07-13 08:03:27.000000 swh.journal-1.3.4/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh/journal/
--rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18355 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     7860 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/serializers.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/swh/journal/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/journal_data.py
--rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/log4j.properties
--rw-r--r--   0 jenkins    (115) docker     (999)    19253 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_kafka_writer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_pytest_plugin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/tests/test_stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.392235 swh.journal-1.3.4/swh/journal/writer/
--rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/inmemory.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-07-13 08:03:27.000000 swh.journal-1.3.4/swh/journal/writer/stream.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-13 08:03:33.388235 swh.journal-1.3.4/swh.journal.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      146 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-13 08:03:33.000000 swh.journal-1.3.4/swh.journal.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-07-13 08:03:27.000000 swh.journal-1.3.4/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-07-25 08:45:38.000000 swh.journal-1.3.5/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      186 2023-07-25 08:45:38.000000 swh.journal-1.3.5/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      848 2023-07-25 08:45:38.000000 swh.journal-1.3.5/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-07-25 08:45:38.000000 swh.journal-1.3.5/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-07-25 08:45:38.000000 swh.journal-1.3.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       15 2023-07-25 08:45:38.000000 swh.journal-1.3.5/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-07-25 08:45:38.000000 swh.journal-1.3.5/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      137 2023-07-25 08:45:38.000000 swh.journal-1.3.5/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-07-25 08:45:38.000000 swh.journal-1.3.5/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-25 08:45:43.916878 swh.journal-1.3.5/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      767 2023-07-25 08:45:38.000000 swh.journal-1.3.5/README.md
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.912878 swh.journal-1.3.5/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.912878 swh.journal-1.3.5/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.912878 swh.journal-1.3.5/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/example-journal-client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      344 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3204 2023-07-25 08:45:38.000000 swh.journal-1.3.5/docs/journal-clients.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      466 2023-07-25 08:45:38.000000 swh.journal-1.3.5/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-07-25 08:45:38.000000 swh.journal-1.3.5/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       59 2023-07-25 08:45:38.000000 swh.journal-1.3.5/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-07-25 08:45:38.000000 swh.journal-1.3.5/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-07-25 08:45:38.000000 swh.journal-1.3.5/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      405 2023-07-25 08:45:38.000000 swh.journal-1.3.5/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-07-25 08:45:43.916878 swh.journal-1.3.5/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2336 2023-07-25 08:45:38.000000 swh.journal-1.3.5/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/swh/journal/
+-rw-r--r--   0 jenkins    (115) docker     (999)      326 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18418 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     7860 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3624 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/serializers.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/swh/journal/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      521 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/journal_data.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      465 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/log4j.properties
+-rw-r--r--   0 jenkins    (115) docker     (999)    19253 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1807 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7988 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_kafka_writer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2183 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_pytest_plugin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3181 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2465 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/tests/test_stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/swh/journal/writer/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2110 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/writer/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1753 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/writer/inmemory.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1156 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/writer/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     9719 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/writer/kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1491 2023-07-25 08:45:38.000000 swh.journal-1.3.5/swh/journal/writer/stream.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-07-25 08:45:43.916878 swh.journal-1.3.5/swh.journal.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1692 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1246 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      146 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-07-25 08:45:43.000000 swh.journal-1.3.5/swh.journal.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1539 2023-07-25 08:45:38.000000 swh.journal-1.3.5/tox.ini
```

### Comparing `swh.journal-1.3.4/.pre-commit-config.yaml` & `swh.journal-1.3.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/CODE_OF_CONDUCT.md` & `swh.journal-1.3.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/LICENSE` & `swh.journal-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/PKG-INFO` & `swh.journal-1.3.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.4
+Version: 1.3.5
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.4/README.md` & `swh.journal-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/docs/example-journal-client.py` & `swh.journal-1.3.5/docs/example-journal-client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/docs/journal-clients.rst` & `swh.journal-1.3.5/docs/journal-clients.rst`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/setup.py` & `swh.journal-1.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/client.py` & `swh.journal-1.3.5/swh/journal/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,23 +296,24 @@
 
         if create_topics:
             topic_list = [
                 NewTopic(topic, 1, 1)
                 for topic in self.subscription
                 if topic not in existing_topics
             ]
-            logger.debug("Creating topics: %s", topic_list)
-            admin_client = AdminClient({"bootstrap.servers": ",".join(brokers)})
-            for topic in admin_client.create_topics(topic_list).values():
-                try:
-                    # wait for topic to be created
-                    topic.result()  # type: ignore[attr-defined]
-                except KafkaException:
-                    # topic already exists
-                    pass
+            if topic_list:
+                logger.debug("Creating topics: %s", topic_list)
+                admin_client = AdminClient({"bootstrap.servers": ",".join(brokers)})
+                for topic in admin_client.create_topics(topic_list).values():
+                    try:
+                        # wait for topic to be created
+                        topic.result()  # type: ignore[attr-defined]
+                    except KafkaException:
+                        # topic already exists
+                        pass
 
         if unknown_types:
             raise ValueError(
                 f"Topic(s) for object types {','.join(unknown_types)} "
                 "are unknown on the kafka broker"
             )
```

### Comparing `swh.journal-1.3.4/swh/journal/pytest_plugin.py` & `swh.journal-1.3.5/swh/journal/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/serializers.py` & `swh.journal-1.3.5/swh/journal/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/journal_data.py` & `swh.journal-1.3.5/swh/journal/tests/journal_data.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_client.py` & `swh.journal-1.3.5/swh/journal/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_inmemory.py` & `swh.journal-1.3.5/swh/journal/tests/test_inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_kafka_writer.py` & `swh.journal-1.3.5/swh/journal/tests/test_kafka_writer.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_pytest_plugin.py` & `swh.journal-1.3.5/swh/journal/tests/test_pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_serializers.py` & `swh.journal-1.3.5/swh/journal/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/tests/test_stream.py` & `swh.journal-1.3.5/swh/journal/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/writer/__init__.py` & `swh.journal-1.3.5/swh/journal/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/writer/inmemory.py` & `swh.journal-1.3.5/swh/journal/writer/inmemory.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/writer/interface.py` & `swh.journal-1.3.5/swh/journal/writer/interface.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/writer/kafka.py` & `swh.journal-1.3.5/swh/journal/writer/kafka.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh/journal/writer/stream.py` & `swh.journal-1.3.5/swh/journal/writer/stream.py`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/swh.journal.egg-info/PKG-INFO` & `swh.journal-1.3.5/swh.journal.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.journal
-Version: 1.3.4
+Version: 1.3.5
 Summary: Software Heritage Journal utilities
 Home-page: https://forge.softwareheritage.org/diffusion/DJNL/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-journal
```

### Comparing `swh.journal-1.3.4/swh.journal.egg-info/SOURCES.txt` & `swh.journal-1.3.5/swh.journal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.journal-1.3.4/tox.ini` & `swh.journal-1.3.5/tox.ini`

 * *Files identical despite different names*

