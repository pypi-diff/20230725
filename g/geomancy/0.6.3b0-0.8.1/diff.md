# Comparing `tmp/geomancy-0.6.3b0.tar.gz` & `tmp/geomancy-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomancy-0.6.3b0.tar", last modified: Mon Jul 24 15:16:26 2023, max compression
+gzip compressed data, was "geomancy-0.8.1.tar", last modified: Tue Jul 25 18:59:09 2023, max compression
```

## Comparing `geomancy-0.6.3b0.tar` & `geomancy-0.8.1.tar`

### file list

```diff
@@ -1,50 +1,71 @@
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.720303 geomancy-0.6.3b0/
--rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.6.3b0/.editorconfig
--rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-20 09:53:51.000000 geomancy-0.6.3b0/.gitignore
--rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.6.3b0/LICENSE.md
--rw-r--r--   0 jlorieau   (501) staff       (20)     6721 2023-07-24 15:16:26.719597 geomancy-0.6.3b0/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)     6324 2023-07-24 15:11:27.000000 geomancy-0.6.3b0/README.md
--rw-r--r--   0 jlorieau   (501) staff       (20)      587 2023-07-20 19:50:56.000000 geomancy-0.6.3b0/Taskfile.yml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.695136 geomancy-0.6.3b0/assets/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1340 2023-07-24 14:40:21.000000 geomancy-0.6.3b0/assets/geomancy.svg
--rw-r--r--   0 jlorieau   (501) staff       (20)     1525 2023-07-24 14:52:00.000000 geomancy-0.6.3b0/assets/geomancy_logo.svg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.696334 geomancy-0.6.3b0/examples/
--rw-r--r--   0 jlorieau   (501) staff       (20)     1273 2023-07-23 19:48:55.000000 geomancy-0.6.3b0/examples/geomancy.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.6.3b0/examples/pyproject.toml
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.697878 geomancy-0.6.3b0/geomancy/
--rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.6.3b0/geomancy/__description__.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      477 2023-07-24 15:12:23.000000 geomancy-0.6.3b0/geomancy/__init__.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.706363 geomancy-0.6.3b0/geomancy/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.6.3b0/geomancy/checks/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)    13168 2023-07-24 01:16:25.000000 geomancy-0.6.3b0/geomancy/checks/base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-23 16:57:03.000000 geomancy-0.6.3b0/geomancy/checks/env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2206 2023-07-24 01:29:48.000000 geomancy-0.6.3b0/geomancy/checks/exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.6.3b0/geomancy/checks/path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     4180 2023-07-24 01:10:18.000000 geomancy-0.6.3b0/geomancy/checks/utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.709133 geomancy-0.6.3b0/geomancy/cli/
--rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.6.3b0/geomancy/cli/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.6.3b0/geomancy/cli/term.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.711183 geomancy-0.6.3b0/geomancy/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.6.3b0/geomancy/config/__init__.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.6.3b0/geomancy/config/config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     5046 2023-07-23 20:54:10.000000 geomancy-0.6.3b0/geomancy/main.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.700497 geomancy-0.6.3b0/geomancy.egg-info/
--rw-r--r--   0 jlorieau   (501) staff       (20)     6721 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/PKG-INFO
--rw-r--r--   0 jlorieau   (501) staff       (20)      877 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/SOURCES.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/dependency_links.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/entry_points.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)       45 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/requires.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-24 15:16:26.000000 geomancy-0.6.3b0/geomancy.egg-info/top_level.txt
--rw-r--r--   0 jlorieau   (501) staff       (20)      791 2023-07-24 15:16:01.000000 geomancy-0.6.3b0/pyproject.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-24 15:16:26.720494 geomancy-0.6.3b0/setup.cfg
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.712195 geomancy-0.6.3b0/tests/
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.716483 geomancy-0.6.3b0/tests/checks/
--rw-r--r--   0 jlorieau   (501) staff       (20)     2968 2023-07-22 17:33:51.000000 geomancy-0.6.3b0/tests/checks/test_base.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.6.3b0/tests/checks/test_env.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1171 2023-07-23 19:38:14.000000 geomancy-0.6.3b0/tests/checks/test_exec.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.6.3b0/tests/checks/test_path.py
--rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.6.3b0/tests/checks/test_utils.py
-drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-24 15:16:26.718207 geomancy-0.6.3b0/tests/config/
--rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.6.3b0/tests/config/config1.toml
--rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.6.3b0/tests/config/test_config.py
--rw-r--r--   0 jlorieau   (501) staff       (20)     1647 2023-07-22 16:20:11.000000 geomancy-0.6.3b0/tests/test_main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.007358 geomancy-0.8.1/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      256 2023-07-20 19:04:04.000000 geomancy-0.8.1/.editorconfig
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1780 2023-07-24 22:25:03.000000 geomancy-0.8.1/.gitignore
+-rw-r--r--   0 jlorieau   (501) staff       (20)      233 2023-07-25 16:40:32.000000 geomancy-0.8.1/.readthedocs.yaml
+-rw-r--r--   0 jlorieau   (501) staff       (20)    35142 2023-07-19 19:00:29.000000 geomancy-0.8.1/LICENSE.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4847 2023-07-25 18:59:09.006869 geomancy-0.8.1/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4431 2023-07-25 16:59:47.000000 geomancy-0.8.1/README.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1571 2023-07-25 18:54:25.000000 geomancy-0.8.1/Taskfile.yml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.979115 geomancy-0.8.1/changelog/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      310 2023-07-25 18:53:41.000000 geomancy-0.8.1/changelog/changelog_template.jinja
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.980955 geomancy-0.8.1/docs/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.982170 geomancy-0.8.1/docs/_static/
+-rw-r--r--   0 jlorieau   (501) staff       (20)    49829 2023-07-25 15:23:09.000000 geomancy-0.8.1/docs/_static/geomancy_logo.png
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1820 2023-07-25 15:22:31.000000 geomancy-0.8.1/docs/_static/geomancy_logo.svg
+-rw-r--r--   0 jlorieau   (501) staff       (20)      736 2023-07-25 18:54:35.000000 geomancy-0.8.1/docs/changelog.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2122 2023-07-25 15:30:06.000000 geomancy-0.8.1/docs/conf.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      458 2023-07-25 18:44:33.000000 geomancy-0.8.1/docs/index.md
+-rw-r--r--   0 jlorieau   (501) staff       (20)      121 2023-07-25 15:07:00.000000 geomancy-0.8.1/docs/quickstart.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.982595 geomancy-0.8.1/docs/usage/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6459 2023-07-25 17:03:06.000000 geomancy-0.8.1/docs/usage/index.md
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.984117 geomancy-0.8.1/examples/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1485 2023-07-24 19:24:24.000000 geomancy-0.8.1/examples/geomancy.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)      512 2023-07-22 13:17:41.000000 geomancy-0.8.1/examples/pyproject.toml
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.985426 geomancy-0.8.1/geomancy/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       59 2023-07-23 20:49:04.000000 geomancy-0.8.1/geomancy/__description__.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      485 2023-07-25 18:43:01.000000 geomancy-0.8.1/geomancy/__init__.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.994141 geomancy-0.8.1/geomancy/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      345 2023-07-24 12:18:52.000000 geomancy-0.8.1/geomancy/checks/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)    11675 2023-07-24 19:29:23.000000 geomancy-0.8.1/geomancy/checks/base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1717 2023-07-24 18:15:32.000000 geomancy-0.8.1/geomancy/checks/env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2426 2023-07-24 15:55:52.000000 geomancy-0.8.1/geomancy/checks/exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1549 2023-07-23 16:57:23.000000 geomancy-0.8.1/geomancy/checks/path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2912 2023-07-24 15:55:58.000000 geomancy-0.8.1/geomancy/checks/python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     5888 2023-07-24 20:38:18.000000 geomancy-0.8.1/geomancy/checks/utils.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2336 2023-07-24 15:55:27.000000 geomancy-0.8.1/geomancy/checks/version.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.995667 geomancy-0.8.1/geomancy/cli/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       42 2023-07-23 11:20:13.000000 geomancy-0.8.1/geomancy/cli/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9027 2023-07-23 16:16:44.000000 geomancy-0.8.1/geomancy/cli/term.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.996880 geomancy-0.8.1/geomancy/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      137 2023-07-22 15:14:01.000000 geomancy-0.8.1/geomancy/config/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     9726 2023-07-22 15:36:57.000000 geomancy-0.8.1/geomancy/config/config.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.998093 geomancy-0.8.1/geomancy/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      164 2023-07-25 01:07:06.000000 geomancy-0.8.1/geomancy/environment/__init__.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4140 2023-07-25 01:16:29.000000 geomancy-0.8.1/geomancy/environment/load_environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6074 2023-07-25 01:48:52.000000 geomancy-0.8.1/geomancy/main.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.988000 geomancy-0.8.1/geomancy.egg-info/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     4847 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/PKG-INFO
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1267 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/SOURCES.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        1 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/dependency_links.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)       47 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/entry_points.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)      124 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/requires.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)        9 2023-07-25 18:59:08.000000 geomancy-0.8.1/geomancy.egg-info/top_level.txt
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2070 2023-07-25 17:48:20.000000 geomancy-0.8.1/pyproject.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)       38 2023-07-25 18:59:09.007465 geomancy-0.8.1/setup.cfg
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:08.999276 geomancy-0.8.1/tests/
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.002973 geomancy-0.8.1/tests/checks/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2955 2023-07-24 19:21:58.000000 geomancy-0.8.1/tests/checks/test_base.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2665 2023-07-23 16:39:02.000000 geomancy-0.8.1/tests/checks/test_env.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     1461 2023-07-24 15:35:23.000000 geomancy-0.8.1/tests/checks/test_exec.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2347 2023-07-23 10:43:50.000000 geomancy-0.8.1/tests/checks/test_path.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2442 2023-07-24 15:31:44.000000 geomancy-0.8.1/tests/checks/test_python.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      828 2023-07-22 11:59:17.000000 geomancy-0.8.1/tests/checks/test_utils.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.004571 geomancy-0.8.1/tests/config/
+-rw-r--r--   0 jlorieau   (501) staff       (20)       73 2023-07-20 16:27:03.000000 geomancy-0.8.1/tests/config/config1.toml
+-rw-r--r--   0 jlorieau   (501) staff       (20)     6468 2023-07-22 15:36:00.000000 geomancy-0.8.1/tests/config/test_config.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)      524 2023-07-25 04:11:09.000000 geomancy-0.8.1/tests/conftest.py
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.005229 geomancy-0.8.1/tests/data/
+-rw-r--r--   0 jlorieau   (501) staff       (20)      159 2023-07-25 01:20:06.000000 geomancy-0.8.1/tests/data/test.env
+drwxr-xr-x   0 jlorieau   (501) staff       (20)        0 2023-07-25 18:59:09.005844 geomancy-0.8.1/tests/environment/
+-rw-r--r--   0 jlorieau   (501) staff       (20)     3181 2023-07-25 04:09:51.000000 geomancy-0.8.1/tests/environment/test_load_environment.py
+-rw-r--r--   0 jlorieau   (501) staff       (20)     2655 2023-07-25 04:08:28.000000 geomancy-0.8.1/tests/test_main.py
```

### Comparing `geomancy-0.6.3b0/.gitignore` & `geomancy-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/LICENSE.md` & `geomancy-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/PKG-INFO` & `geomancy-0.8.1/docs/usage/index.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,170 +1,288 @@
-Metadata-Version: 2.1
-Name: geomancy
-Version: 0.6.3b0
-Summary: Geomancy validates deployment and development environments
-Author: Justin Lorieau
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
-<img src="https://raw.githubusercontent.com/jlorieau/geomancy/main/assets/geomancy_logo.svg" alt="geomancy" height="120" />
-
-[![pypi version](https://img.shields.io/pypi/v/geomancy.svg)](https://pypi.org/project/geomancy/)
-[![python versions](https://img.shields.io/pypi/pyversions/geomancy.svg)](https://pypi.org/project/geomancy/)
-[![Black formatting](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-
-The ``geomancy`` tool makes it easy to check and validate environments, such
-as development, testing and production.
-
-Currently, ``geomancy`` can check:
-- [environment variables](#checkenv) are properly set
-- [file and directory paths](#checkpath) exist
-- [executables](#checkexec) are available and, optionally, of the correct version
-- [groups of checks](#check-groups) with conditional evaluation
-- parameter values with substitution of environment variables.
-  ex: ``checkPath: {HOME}/.geomancy.toml``
-
-The following is an example ``geomancy`` run with an example checks file.
-
-```shell
-$ geo examples/geomancy.toml
-========================= examples/geomancy.toml =========================
-    checks (10 checks)
-[✔]   Environment (2 checks)
-[✔]     Check environment variable '{PATH}'...passed
-[✔]     Check environment variable '{USER}'...passed
-      Paths (4 checks)
-[✔]     ChecksFile (3 checks)
-[✔]       Check path 'examples/geomancy.toml'...passed
-[✔]       Check path 'examples/pyproject.toml'...passed
-[!]       Check path '.missing__.txt'...missing
-[✔]   Executables (1 checks)
-[✔]     Check executable 'python3>=3.11'...passed
-========================= 11 checks passed in 0.00s ======================
-```
-
-## Usage
-1. Create a file containing checks. Either
-
-   - ``.geomancy.toml`` in the project root. See the ``examples`` directory for
-     examples.
-
-   or
-
-   - ``pyproject.toml`` with checks and config in the ``[tool.geomancy]`` section.
-
-2. Run the geo
-
-   ```shell
-   $ geo
-   ```
+# Usage
 
 ## Format
 
-### Check Groups
+The checks file is formatted in [TOML](https://toml.io/en/), and it contains a
+listing of checks and, optionally, configuration options for ``geomancy``.
 
-Check groups are sections which contain one or more sub-checks.
+### Filenames
 
-| name      | description                                                                                                                                     |
-|:----------|:------------------------------------------------------------------------------------------------------------------------------------------------|
-| desc      | _(Optional)_ The description for the check section                                                                                              |
-| condition | _(Optional)_ Either ``'all'`` to require that all sub-checks pass or ``'any'`` to require that only one sub-check passes.<br>Default: ``'all'`` |
+The checks file may be a dedicated file for ``geomancy``, such as a
+``.geomancy.toml`` file or a ``geomancy.toml`` file in the project root
+directory, or it may be incorporated as part of a ``pyproject.toml`` file
+under the ``[tool.geomancy]`` section.
 
-##### Examples
+::::{tab-set}
 
-The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
-``Pyproject``.
+:::{tab-item} .geomancy.toml
+```toml
+[checks.Username]
+desc = "The current username"
+checkEnv = "{USER}"
+regex = "[a-z_][a-z0-9_-]*[$]?"
+```
+:::
+
+:::{tab-item} pyproject.toml
+```toml
+[tool.geomancy.checks.Username]
+desc = "The current username"
+checkEnv = "{USER}"
+regex = "[a-z_][a-z0-9_-]*[$]?"
+```
+:::
+
+::::
+
+### Nesting and Listing Checks
+
+Checks can be grouped into sections of related checks, and the pass condition
+for child checks can be customized.
+
+::::{tab-set}
+
+:::{tab-item} .geomancy.toml
+By default, all child checks must pass for the parent check to pass.
+In this example, the parent check, ``ChecksFile``, may pass if any of the
+3 child checks pass--either ``Geomancy``, ``Pyproject`` or ``missing``. This
+condition is specified by ``subchecks = "any"`` option.
 
 ```toml
 [checks.ChecksFile]
-    desc = "Checks that at least one checks file exists"
-    condition = "any"
+desc = "Checks that at least one checks file exists"
+subchecks = "any"
 
     [checks.ChecksFile.Geomancy]
     desc = "Check for 'geomancy.toml' file"
     checkPath = "examples/geomancy.toml"
     type = "file"
 
     [checks.ChecksFile.Pyproject]
     desc = "Check for 'pyproject.toml' file"
     checkPath = "examples/pyproject.toml"
     type = "file"
+
+    [checks.ChecksFile.missing]
+    desc = "Check a missing file"
+    checkPath = ".missing__.txt"
+    type = "file"
 ```
+:::
+
+::::
 
-The following is the same check group, but in abbreviated format.
+### Configuration
+Checks files may optionally include configuration settings for ``geomancy``.
+These are specifid under the ``[config]`` section or the
+``[tool.geomancy.config]`` section for ``pyproject.toml`` files.
 
+::::{tab-set}
+
+:::{tab-item} .geomancy.toml
 ```toml
-[checks.ChecksFile]
-    condition = "any"
+[config]
+  [config.CHECKBASE]
+  ENV_SUBSTITUTE_DEFAULT=true
+```
+:::
 
-    Geomancy = {checkPath = "examples/geomancy.toml", type = "file"}
-    Pyproject = {checkPath = "examples/pyproject.toml", type = "file"}
+:::{tab-item} pyproject.toml
+```toml
+[tool.geomancy.config]
+  [tool.geomancy.config.CHECKBASE]
+  ENV_SUBSTITUTE_DEFAULT=true
 ```
+:::
+::::
+
+:::{tip}
+All configuration options and their defaults can be listed in
+[TOML](https://toml.io/en/) format using the ``geo --config`` command.
+:::
+
 
-### Checks
 
-#### checkEnv
+## Checks
+
+The following describes the various checks and their options.
+
+### checkEnv
 
 Check the existence and, optionally, the value of an environment variable.
 
-| name      | description                                                                                                          |
-|:----------|:---------------------------------------------------------------------------------------------------------------------|
-| checkEnv  | Environment variable to check, wrapped in curly braces for substitution. <br>__aliases__: ``checkEnv``, ``CheckEnv`` |
-| desc      | _(Optional)_ The description for the check                                                                           |
-| regex     | _(Optional)_ A regular expression to check against the environment variable value                                    |
+:checkEnv: Environment variable to check, wrapped in curly braces for
+    substitution. <br>
+    __aliases__: ``checkEnv``, ``CheckEnv``
+:desc: _(Optional)_ The description for the check
+:regex: _(Optional)_ A regular expression to check against the environment
+    variable value
 
-##### Examples
+::::{tab-set}
 
+:::{tab-item} Example 1
 ```toml
 [checks.Environment.Username]
 desc = "The current username"
 checkEnv = "{USER}"
 regex = "[a-z_][a-z0-9_-]*[$]?"
 ```
+:::
+
+:::{tab-item} Example 2 (abbreviated)
+```toml
+[checks.Environment]
+Username = {checkEnv = "{USER}", regex="[a-z_][a-z0-9_-]*[$]?"}
+```
+:::
 
-#### checkExec
+::::
+
+
+### checkExec
 
 Check the existence and, optionally, the version of available executables or
 commands.
 
-| name      | description                                                                                                                                   |
-|:----------|:----------------------------------------------------------------------------------------------------------------------------------------------|
-| checkExec | Executable to check. Additionally, an optional version check can be added with a test operator. <br>__aliases__: ``checkExec``, ``CheckExec`` |
-| desc      | _(Optional)_ The description for the check                                                                                                    |
+:checkExec: Executable to check. Additionally, an optional version check
+    can be added with a test operator. <br>
+    __aliases__: ``checkExec``, ``CheckExec``
+:desc: _(Optional)_ The description for the check
 
-##### Examples
+::::{tab-set}
 
+:::{tab-item} Example 1
 ```toml
 [checks.Executables.Ls]
 desc = "List files"
 checkExec = "ls"
 ```
+:::
 
+:::{tab-item} Example 2 (with version)
 ```toml
 [checks.Executables.Python]
 desc = "Python interpreter (version 3.11 or higher)"
 checkExec = "python3>=3.11"
 ```
+:::
+
+:::{tab-item} Example 3 (abbreviated)
+```toml
+[checks.Executables]
+Python = {checkExec = "python3>=3.11"}
+```
+:::
+
+::::
 
-#### checkPath
 
-Check the existence and type of a path.
+### checkPath
 
-| name      | description                                                                                                                                    |
-|:----------|:-----------------------------------------------------------------------------------------------------------------------------------------------|
-| checkPath | Path to check, which may include environment variables wrapped in curly braces for substitution. <br>__aliases__: ``checkPath``, ``CheckPath`` |
-| desc      | _(Optional)_ The description for the check                                                                                                     |
-| type      | _(Optional)_ Additionally check whether the path corresponds to a valid ``'file'`` or ``'dir'``.                                               |
+Check the existence and, optionally, the type of a path.
 
-##### Examples
+:checkPath: Path to check, which may include environment variables wrapped
+    in curly braces for substitution. <br>
+    __aliases__: ``checkPath``, ``CheckPath``
+:desc: _(Optional)_ The description for the check
+:type: _(Optional)_ Additionally check whether the path corresponds to a
+    valid ``'file'`` or ``'dir'``.
 
+::::{tab-set}
+
+:::{tab-item} Example 1
 ```toml
 [checks.Environment.Pyproject]
 desc = "A project's pyprojectfile"
 checkPath = "./pyproject.toml"
 path_type = "file"
 ```
+:::
+
+:::{tab-item} Example 2 (abbreviated)
+```toml
+[checks.Environment]
+Pyproject = {checkPath = "./pyproject.toml", path_type = "file"}
+```
+:::
+
+::::
+
+### checkPythonPkg
+
+Checks whether the python package is installed and, optionally, check its
+version.
+
+:checkPythonPkg: Python package to check. Additionally, an optional version
+    check can be added with a test operator. <br>
+    __aliases__: ``checkPythonPkg``, ``CheckPythonPkg``,
+    ``checkPythonPackage``, ``CheckPythonPackage``
+:desc: _(Optional)_ The description for the check
+
+::::{tab-set}
+
+:::{tab-item} Example 1
+```toml
+[checks.PythonPackages.geomancy]
+desc = "Geomancy python package"
+checkPythonPkg = "geomancy>=0.1"
+```
+:::
+
+:::{tab-item} Example 2 (abbreviated)
+```toml
+[checks.PythonPackages]
+geomancy = {checkPythonPkg = "geomancy>=0.1"}
+```
+:::
+
+::::
+
+
+### Check Groups
+
+Check groups are sections which contain one or more child checks.
+
+:desc: _(Optional)_ The description for the check section
+:subchecks: _(Optional)_ Either ``'all'`` to require that all sub-checks
+    pass or ``'any'`` to require that only one sub-check passes.<br>
+    Default: ``'all'``<br>
+    __aliases__: ``condition``
+
+::::{tab-set}
+
+:::{tab-item} Example 1
+The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+``Pyproject``.
+
+```toml
+[checks.ChecksFile]
+desc = "Checks that at least one checks file exists"
+subchecks = "any"
+
+    [checks.ChecksFile.Geomancy]
+    desc = "Check for 'geomancy.toml' file"
+    checkPath = "examples/geomancy.toml"
+    type = "file"
+
+    [checks.ChecksFile.Pyproject]
+    desc = "Check for 'pyproject.toml' file"
+    checkPath = "examples/pyproject.toml"
+    type = "file"
+```
+:::
+
+:::{tab-item} Example 2 (abbreviated)
+The following is a check group ``ChecksFile`` with 2 checks, ``Geomancy`` and
+``Pyproject``, in abbreviated format.
+
+```toml
+[checks.ChecksFile]
+subchecks = "any"
+
+Geomancy = {checkPath = "examples/geomancy.toml", type = "file"}
+Pyproject = {checkPath = "examples/pyproject.toml", type = "file"}
+```
+
+:::
+
+::::
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `geomancy-0.6.3b0/examples/geomancy.toml` & `geomancy-0.8.1/examples/geomancy.toml`

 * *Files 14% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     regex = "[a-z_][a-z0-9_-]*[$]?"
 
 [checks.Paths]
 desc = "Checks the existence of needed files and directories"
 
     [checks.Paths.ChecksFile]
     desc = "Checks that at least one checks file exists"
-    condition = "any"
+    subchecks = "any"
 
         [checks.Paths.ChecksFile.Geomancy]
         desc = "Check for 'geomancy.toml' file"
         checkPath = "examples/geomancy.toml"
         type = "file"
 
         [checks.Paths.ChecksFile.Pyproject]
@@ -41,7 +41,15 @@
 
 [checks.Executables]
 desc = "Check the availability of commands and their versions"
 
     [checks.Executables.Python]
     desc = "Python interpreter"
     checkExec = "python3>=3.11"
+
+[checks.PythonPackages]
+desc = "Check the presence and, optional, the version of python packages"
+
+    [checks.PythonPackages.geomancy]
+    desc = "Geomancy python package"
+    checkPythonPkg = "geomancy>=0.1"
+
```

### Comparing `geomancy-0.6.3b0/examples/pyproject.toml` & `geomancy-0.8.1/examples/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/geomancy/checks/base.py` & `geomancy-0.8.1/geomancy/checks/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Abstract base class for checks
 """
 import typing as t
-from abc import ABC, abstractmethod
+from abc import ABC
 from inspect import isabstract
 from collections import namedtuple
 from time import process_time
 
-from .utils import sub_env, name_and_version, all_subclasses
+from .utils import sub_env, all_subclasses, pop_first
 from ..config import Parameter
 from ..cli import Term
 
-__all__ = ("CheckBase", "CheckVersion", "CheckException", "CheckResult")
+__all__ = ("CheckBase", "CheckException", "CheckResult")
 
 
 class CheckException(Exception):
     """Exception raised when an error is encountered in the setup of a check."""
 
 
 # Storage class for the results of checks
@@ -30,92 +30,95 @@
 
     # Description of the check
     desc: str = ""
 
     # The message to print during the check.
     msg: str = "{check.name}"
 
-    # A list of sub checks
-    sub_checks: t.List["CheckBase"]
+    # A list of children checks
+    children: t.List["CheckBase"]
 
     # Alternative names for the class
     aliases: t.Optional[t.Tuple[str, ...]] = None
 
-    # The check (and sub-checks) are enabled
+    # This check (and children) are enabled
     enabled: bool = True
 
     # If True (default), environment variables in variable_name or
     # variable_value are substituted with the values of other environment
     # variables.
     env_substitute: bool
 
-    # The condition for sub-check results to be considered a pass
+    # The condition for children results to be considered a pass
     condition: t.Callable = all
+    condition_aliases = ("condition", "subchecks")  # other names for variable
 
     # The default value for env_substitute
     env_substitute_default = Parameter("CHECKBASE.ENV_SUBSTITUTE_DEFAULT", default=True)
+    env_substitute_aliases = ("env_substitute",)  # other names for variable
 
     # The maximum recursion depth of the load function
     max_level = Parameter("CHECKBASE.MAX_LEVEL", default=10)
 
     def __init__(
         self,
         name: str,
         value: t.Optional[str] = None,
         desc: str = "",
-        condition: t.Optional[str] = None,
-        env_substitute: t.Optional[bool] = None,
-        sub_checks: t.Optional[list["CheckBase", ...]] = None,
+        children: t.Optional[list["CheckBase", ...]] = None,
+        **kwargs,
     ):
         self.name = name
         self.value = value
         self.desc = desc
+        self.children = list(children) if children is not None else []
+
+        # Parse kwargs, which may use different aliases
+        condition = pop_first(kwargs, *self.condition_aliases, default=None)
         self.env_substitute = (
-            env_substitute
-            if env_substitute is not None
-            else self.env_substitute_default
+            pop_first(kwargs, *self.env_substitute_aliases, default=None)
+            or self.env_substitute_default
         )
-        self.sub_checks = list(sub_checks) if sub_checks is not None else []
 
         # Make sure the condition values are allowed
         if condition is None:
             pass
         elif condition in ("all", "All", "ALL"):
             self.condition = all
         elif condition in ("any", "Any", "ANY"):
             self.condition = any
         else:
             raise CheckException(
                 f"The condition '{condition}' should be either 'all' or 'any'."
             )
 
         # Check attributes
-        msg = "All sub-checks should be instances of CheckBase"
-        assert all(isinstance(sc, CheckBase) for sc in self.sub_checks), msg
+        msg = "All children should be instances of CheckBase"
+        assert all(isinstance(sc, CheckBase) for sc in self.children), msg
 
     def __repr__(self):
         return f"{self.__class__.__name__}({self.name})"
 
     def __len__(self):
-        """The number of sub-checks"""
-        return len(self.sub_checks)
+        """The number of children"""
+        return len(self.children)
 
     @property
     def count(self, all: bool = True) -> int:
-        """The number of sub-checks
+        """The number of children
 
         Parameters
         ----------
         all
-            If True, count all the immediate and nested level sub-checks.
-            If False, only count the immediate level sub-checks.
+            If True, count all the immediate and nested level children.
+            If False, only count the immediate level children.
         """
         # flatten() returns this check, so the count is subtracted by 1 to only
         # count sub-checks
-        return len(self.flatten()) - 1 if all else len(self.sub_checks)
+        return len(self.flatten()) - 1 if all else len(self.children)
 
     @property
     def value(self) -> t.Any:
         """Check's value with optional environment substitution"""
         if self.env_substitute and self.raw_value is not None:
             subbed = sub_env(self.raw_value)
             return subbed if subbed is not None else self.raw_value
@@ -124,27 +127,27 @@
 
     @value.setter
     def value(self, v):
         self.raw_value = str(v) if v is not None else None
 
     @property
     def is_collection(self) -> bool:
-        """Evaluate whether this is a collection check--i.e. it's only a check that
-        holds other check groups (BaseCheck instances).
+        """Evaluate whether this is a collection check--i.e. it's only a
+        check that holds other check groups (BaseCheck instances).
 
-        Collection checks have headings that are printed before the results of the
-        sub-checks are evaluated.
+        Collection checks have headings that are printed before the results of
+        the children are evaluated.
         """
         collection_clses = (CheckBase,)
         return self.__class__ in collection_clses and all(
-            sub.__class__ in (CheckBase,) for sub in self.sub_checks
+            child.__class__ in (CheckBase,) for child in self.children
         )
 
     def check(self, level: int = 0) -> CheckResult:
-        """Performs the checks and sub-checks.
+        """Performs the checks of this check and of children.
 
         Parameters
         ----------
         level
             The current depth level of the check
 
         Returns
@@ -159,26 +162,26 @@
         start_time = None
         if level == 0:
             # Top level heading
             term.p_h1(msg=msg, level=level)
             start_time = process_time()
         elif self.is_collection:
             # Collection checks print right away since we don't need to wait to
-            # see the results of "check" for sub_checks
+            # see the results of "check" for children
             term.p_h2(
                 msg=msg,
                 level=level,
                 status=f" ({self.count} checks)",
                 color_status=term.RESET,
             )
 
-        # Run all sub-checks
+        # Run all children checks
         results = []
-        for sub_check in self.sub_checks:
-            result = sub_check.check(level=level + 1)
+        for child in self.children:
+            result = child.check(level=level + 1)
             results.append(result)
 
         # Determine if this check passed based on the condition
         passed = self.condition(result.passed for result in results)
 
         # Print this check's results
         if passed and not self.is_collection:
@@ -201,24 +204,25 @@
         for result in results:
             if result.msg == "":
                 # This result has already been handled and printed
                 continue
             elif result.passed:
                 term.p_pass(msg=result.msg, status=result.status, level=level + 1)
             elif passed:
-                # If the sub-check failed but this check passed, then it's a
-                # warning.
+                # If the child check failed but this check passed, then it's a
+                # warning
                 term.p_warn(msg=result.msg, status=result.status, level=level + 1)
             else:
-                # If the sub-check failed and this check failed, then it's a fail.
+                # If the child check failed and this check failed, then it's a
+                # fail
                 term.p_fail(msg=result.msg, status=result.status, level=level + 1)
 
         # Print terminal information if this is the root check
         if level == 0:
-            msg = f"{self.count} checks {'passed' if passed else 'failed'}"
+            msg = f"{'PASSED' if passed else 'FAILED'}. {self.count} checks"
 
             # Add timing info, if available
             if start_time is not None:
                 total_time = process_time() - start_time
                 msg += f" in {total_time:.2f}s"
 
             # Determine the message color
@@ -226,25 +230,25 @@
 
             # Print the message
             term.p_h1(msg, color_msg=color_msg)
 
         return CheckResult(passed=passed, msg="", status="")
 
     def flatten(self) -> t.List["CheckBase"]:
-        """Return a flattened list of this check (first item) and all
-        sub checks."""
+        """Return a flattened list of this check (first item) and children
+        checks"""
         flattened = [self]
-        for sub_check in self.sub_checks:
-            flattened += sub_check.flatten()
+        for child in self.children:
+            flattened += child.flatten()
         return flattened
 
     @classmethod
     def types_dict(cls) -> t.Dict[str, t.Type]:
-        """Return all the types and subtypes of Checks in a dict."""
-        # Retrieve the base class (BaseCheck) and subclasses
+        """Return all the instantiatable CheckBase types in a dict."""
+        # Retrieve the base class (BaseCheck) and children classes
         cls_types = [cls] + list(all_subclasses(cls))
 
         # Create a dict with the class name string (key) and the class type
         # (value)
         d = dict()
         for cls_type in cls_types:
             # Skip abstract classes, which can't be instantiated
@@ -257,15 +261,14 @@
             # Add class name aliases
             aliases = cls_type.aliases if cls_type.aliases is not None else ()
             for alias in aliases:
                 # Aliases should not create name collisions
                 assert alias not in d, f"Duplicate alias name '{alias}'"
 
                 d[alias] = cls_type
-        print(d)
         return d
 
     @classmethod
     def load(
         cls, d: dict, name: str, level: int = 1, max_level: t.Optional[int] = None
     ) -> t.Union["CheckBase", None]:
         """Load checks from a dict.
@@ -314,15 +317,15 @@
 
             # Get the other kwargs
             kwargs = {k: v for k, v in d.items() if k != check_type}
 
             # Create and return the check_type
             return matching_cls(name, value, **kwargs)
 
-        # Otherwise, try parsing the sub_checks
+        # Otherwise, try parsing the children
         items = d.items()
         found_checks = []  # Values parsed into CheckBase objects
         other_d = dict()  # All other values
         for key, value in items:
             if not isinstance(value, dict):
                 other_d[key] = value
                 continue
@@ -334,64 +337,13 @@
             # Replace the value withe CheckBase instance, if it was parsed correctly
             # Otherwise, just place it in the parsed_dict.
             if isinstance(return_value, CheckBase):
                 found_checks.append(return_value)
             else:
                 other_d[key] = value
 
-        # No sub-checks found; nothing else to do
+        # No child checks found; nothing else to do
         if len(found_checks) == 0:
             return None
 
         # Create a check grouping, first, by parsing the other arguments
-        return CheckBase(name=name, sub_checks=found_checks, **other_d)
-
-
-class CheckVersion(CheckBase):
-    """An abstract Check for package and program versions"""
-
-    @property
-    def value(
-        self,
-    ) -> t.Tuple[
-        t.Union[str, None], t.Union[t.Callable, None], t.Union[t.Tuple[int], None]
-    ]:
-        """Get the package name, comparison operator and version tuple."""
-        value = CheckBase.value.fget(self)
-        name, op, version = name_and_version(value)
-        return name, op, version
-
-    @value.setter
-    def value(self, v):
-        CheckBase.value.fset(self, v)
-
-    @abstractmethod
-    def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
-        """Get the current version, or None if it can't be found."""
-        return None
-
-    def check(self, level: int = 0) -> CheckResult:
-        """Check whether the current version is compatible with the version
-        specified in the value."""
-        name, op, version = self.value
-        current_version = self.get_current_version()
-        passed = False
-
-        if name is None:
-            status = "missing"
-        else:
-            if version is not None and current_version is None:
-                status = "present but current version unknown"
-            elif (
-                version is not None
-                and current_version is not None
-                and op is not None
-                and not op(current_version, version)
-            ):
-                status = f"version={'.'.join(map(str, current_version))}"
-            else:
-                status = "passed"
-                passed = True
-
-        return CheckResult(
-            passed=passed, msg=self.msg.format(check=self), status=status
-        )
+        return CheckBase(name=name, children=found_checks, **other_d)
```

### Comparing `geomancy-0.6.3b0/geomancy/checks/env.py` & `geomancy-0.8.1/geomancy/checks/env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/geomancy/checks/exec.py` & `geomancy-0.8.1/geomancy/checks/exec.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 """
 Checks for executables
 """
 import typing as t
 from shutil import which
 import subprocess
 
-from .base import CheckVersion
+from .version import CheckVersion
 from .utils import version_to_tuple
 from ..config import Parameter
 
 __all__ = ("CheckExec",)
 
 
 class CheckExec(CheckVersion):
     """Check for the presence and version of executables"""
 
-    # The message for checking environment variables
+    # The executable may exist and be installed, but get_current_version
+    # may not be able to identify the current version
+    require_current_version = False
+
+    # The message for checking executables
     msg = Parameter(
         "CHECKEXEC.MSG",
         default="Check executable '{check.raw_value}'...",
     )
 
     # Alternative names for the class
     aliases = ("checkExec",)
@@ -39,14 +43,15 @@
         return cmd_name, op, version
 
     @value.setter
     def value(self, v):
         CheckVersion.value.fset(self, v)
 
     def get_current_version(self) -> t.Union[None, t.Tuple[int]]:
+        """Try to get the version tuple for the executable."""
         cmd_name, op, version = self.value
 
         if cmd_name is None:  # command not found
             return None
 
         for args in (  # Different commands to try for versions
             (cmd_name, "-V"),
```

### Comparing `geomancy-0.6.3b0/geomancy/checks/path.py` & `geomancy-0.8.1/geomancy/checks/path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/geomancy/checks/utils.py` & `geomancy-0.8.1/geomancy/checks/utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 import typing as t
 import os
 import operator
 import re
 
 __all__ = ("all_subclasses", "sub_env", "version_to_tuple", "name_and_version")
 
+__missing__ = object()  # used an argument for missing values
+
 
 def all_subclasses(cls) -> t.List[t.Type]:
     """Retrieve all subclasses, sub-subclasses and so on for a class
 
     Parameters
     ----------
     cls : Type
@@ -49,14 +51,80 @@
         o_type = type(obj)
         items = obj.items() if hasattr(obj, "items") else obj
         return o_type(sub_env(i) for i in items)
     else:
         return obj
 
 
+def pop_first(d: dict, *keys, del_remaining: bool = True, default: t.Any = __missing__):
+    """Pop the first key found in the dict.
+
+    Parameters
+    ----------
+    d
+        The dict to search for keys to pop
+    *keys
+        The list of keys to search
+    del_remaining
+        Delete the remaining keys from the dict
+    default
+        Return this value if a key isn't found. If not specified, a KeyError
+        is raised
+
+    Returns
+    -------
+    value
+        The value for the first matching key
+
+    Raises
+    ------
+    KeyError
+        If none of the keys were found and a default wasn't found
+
+    Examples
+    --------
+    >>> pop_first({'a': 1, 'b': 2, 'c': 3}, 'b', 'a')
+    2
+    >>> pop_first({'a': 1, 'b': 2, 'c': 3}, 'a', 'b')
+    1
+    >>> pop_first({'a': 1, 'b': 2, 'c': 3}, 'e', default='missing')
+    'missing'
+    >>> d = {'a1': 1, 'a2': 2, 'b': 3}
+    >>> pop_first(d, 'a1', 'a2')
+    1
+    >>> print(d)
+    {'b': 3}
+    >>> pop_first(d, 'a1')
+    Traceback (most recent call last):
+        ...
+    KeyError: "Could not find any of the keys: ('a1',)"
+    """
+    value = __missing__
+
+    # Find the first key
+    for key in keys:
+        value = d.pop(key, __missing__)
+        if value is not __missing__:
+            break
+
+    # Del remaining
+    if del_remaining:
+        extra_keys = [key for key in keys if key in d]
+        for k in extra_keys:
+            del d[k]
+
+    # Return a value or raise an exception
+    if value is not __missing__:
+        return value
+    elif default is not __missing__:
+        return default
+    else:
+        raise KeyError(f"Could not find any of the keys: {keys}")
+
+
 def version_to_tuple(version: str) -> t.Union[t.Tuple[int], None]:
     """Convert a semantic version string to a tuple of integers.
 
     Parameters
     ----------
     version
         String with the version number. e.g. '1.4.3]
@@ -78,15 +146,15 @@
     >>> version_to_tuple('1.3')
     (1, 3)
     >>> version_to_tuple('v0.1.3')
     (0, 1, 3)
     >>> version_to_tuple('1.2beta')
     (1, 2)
     """
-    version_match = re.search(r"([\d.]{2,}|\d+)", version)  # Capture the version
+    version_match = re.search(r"([\d\.]{2,}|\d+)", version)  # Capture the version
     if version_match is None:
         return None
     version = version_match.group().split(".")  # Split the version string at "."
     return tuple(map(int, version))  # Convert to a tuple of ints
 
 
 def name_and_version(
@@ -121,17 +189,17 @@
     >>> name_and_version('jinja2>=2.10')
     ('jinja2', <built-in function ge>, (2, 10))
     >>> name_and_version('geo>=0.4.0a')
     ('geo', <built-in function ge>, (0, 4, 0))
     """
 
     m = re.search(
-        r"([\w.\-_]+)"  # match package name
+        r"([\w\.\-_]+)"  # match package name
         r"\s*(==|>=|<=|>|<|!=)?\s*"  # operator
-        r"([\d\w.]+)?",  # version number
+        r"([\d\w\.]+)?",  # version number
         string,
     )
 
     if m is None:
         # The string couldn't be parsed
         return None, None, None
```

### Comparing `geomancy-0.6.3b0/geomancy/cli/term.py` & `geomancy-0.8.1/geomancy/cli/term.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/geomancy/config/config.py` & `geomancy-0.8.1/geomancy/config/config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/geomancy/main.py` & `geomancy-0.8.1/geomancy/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import logging
 from pathlib import Path
 import tomllib
 
 from . import get_version
 from .config import Config
 from .checks import CheckBase
+from .environment import load_env
 
 __description__ = (Path(__file__).parent / "__description__.txt").read_text().strip()
 
 logger = logging.getLogger(__name__)  # Create a default logger
 config = Config()  # Set up config defaults for the CLI
 
 # Set current version
@@ -64,14 +65,27 @@
         "--version",
         action="version",
         version=f"%(prog)s " + get_version(),
         help="Print the current version",
     )
     parser.add_argument("-d", "--debug", action="store_true", help="Enable debug mode")
     parser.add_argument(
+        "-e",
+        "--env",
+        action="append",
+        type=filepath,
+        help="Optional environment file(s) to load",
+    )
+    parser.add_argument(
+        "--overwrite",
+        action="store_true",
+        default=False,
+        help="Overwrite environment variables from files",
+    )
+    parser.add_argument(
         "--disable-color", action="store_true", help="Disable colors in the terminal"
     )
     parser.add_argument("--config", action="store_true", help="Print default config")
     parser.add_argument(
         "checks_files",
         type=filepath,
         nargs="*",
@@ -139,39 +153,57 @@
             config.update(config_section)
 
         # Load the rest into a root CheckBase
         check = CheckBase.load(d, name=str(checks_file))
         if check is not None:
             checks.append(check)
 
+    # Create a root check, if there are a lot of checks
+    if len(checks) > 1:
+        checks = [CheckBase(name="Multiple files", sub_checks=checks)]
+
     # Run the checks
     return all(check.check() for check in checks)
 
 
-def action_config(args) -> bool:
-    """Handle execution of the 'config' sub-command"""
-    config.pprint_toml()
-    return True
+def action_env(args, parser) -> int:
+    """Hand the environment files (-e) options"""
+    # The '--overwrite' flag only makes sense if environment files (-e) are
+    # specified
+    if args.overwrite and args.env is None:
+        parser.error(
+            f"The --overwrite flag can only be used when environment files "
+            f"(--env) are specified"
+        )
+
+    env_files = args.env if args.env is not None else []
+    count = 0
+    for filepath in env_files:
+        count += load_env(filepath, overwrite=args.overwrite)
+    return count
 
 
 def main_cli(args: t.Optional[t.List[str]] = None):
     # Parse the CLI arguments
     parser = setup_parser()
     args = parser.parse_args(args)  # parse root parser args
 
     # Setup the default logger
     setup_logging(debug=args.debug)
     logger.debug(f"CLI parsed args: {args}")
 
     # Process the --config flag
     if args.config:
-        action_config(args)
+        config.pprint_toml()
         exit(0)
 
     # Process the --disable-color flag
     if args.disable_color:
         config.TERM.USE_COLOR = False
 
+    # Process the -e/--env files and --overwrite
+    action_env(args=args, parser=parser)
+
     # Process the checks
     result = action_check(args)
     if result is None:
         parser.print_help()
```

### Comparing `geomancy-0.6.3b0/geomancy.egg-info/SOURCES.txt` & `geomancy-0.8.1/geomancy.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 .editorconfig
 .gitignore
+.readthedocs.yaml
 LICENSE.md
 README.md
 Taskfile.yml
 pyproject.toml
-assets/geomancy.svg
-assets/geomancy_logo.svg
+changelog/changelog_template.jinja
+docs/changelog.md
+docs/conf.py
+docs/index.md
+docs/quickstart.md
+docs/_static/geomancy_logo.png
+docs/_static/geomancy_logo.svg
+docs/usage/index.md
 examples/geomancy.toml
 examples/pyproject.toml
 geomancy/__description__.txt
 geomancy/__init__.py
 geomancy/main.py
 geomancy.egg-info/PKG-INFO
 geomancy.egg-info/SOURCES.txt
@@ -18,20 +25,28 @@
 geomancy.egg-info/requires.txt
 geomancy.egg-info/top_level.txt
 geomancy/checks/__init__.py
 geomancy/checks/base.py
 geomancy/checks/env.py
 geomancy/checks/exec.py
 geomancy/checks/path.py
+geomancy/checks/python.py
 geomancy/checks/utils.py
+geomancy/checks/version.py
 geomancy/cli/__init__.py
 geomancy/cli/term.py
 geomancy/config/__init__.py
 geomancy/config/config.py
+geomancy/environment/__init__.py
+geomancy/environment/load_environment.py
+tests/conftest.py
 tests/test_main.py
 tests/checks/test_base.py
 tests/checks/test_env.py
 tests/checks/test_exec.py
 tests/checks/test_path.py
+tests/checks/test_python.py
 tests/checks/test_utils.py
 tests/config/config1.toml
-tests/config/test_config.py
+tests/config/test_config.py
+tests/data/test.env
+tests/environment/test_load_environment.py
```

### Comparing `geomancy-0.6.3b0/tests/checks/test_base.py` & `geomancy-0.8.1/tests/checks/test_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 
 
 def test_check_base_flatten():
     """Test the CheckBase.flatten() method"""
     # Create a CheckBase tree
     sub11 = CheckBase(name="sub11")
     sub12 = CheckBase(name="sub12")
-    sub1 = CheckBase(name="sub1", sub_checks=[sub11, sub12])
+    sub1 = CheckBase(name="sub1", children=[sub11, sub12])
     sub2 = CheckBase(name="sub2")
-    root = CheckBase(name="root", sub_checks=[sub1, sub2])
+    root = CheckBase(name="root", children=[sub1, sub2])
 
     # Check the flattened tree
     flattened = root.flatten()
 
     assert len(flattened) == 5
     assert flattened[0] == root
     assert flattened[1] == sub1
@@ -89,12 +89,12 @@
 
     # Validate check values
     assert flattened[0].value is None
     assert flattened[1].value is None
     assert flattened[2].value == "VAR1"
     assert flattened[3].value == "VAR2"
 
-    # Validate sub_check entries
-    assert flattened[0].sub_checks == [flattened[1]]
-    assert flattened[1].sub_checks == [flattened[2], flattened[3]]
-    assert flattened[2].sub_checks == []
-    assert flattened[3].sub_checks == []
+    # Validate children entries
+    assert flattened[0].children == [flattened[1]]
+    assert flattened[1].children == [flattened[2], flattened[3]]
+    assert flattened[2].children == []
+    assert flattened[3].children == []
```

### Comparing `geomancy-0.6.3b0/tests/checks/test_env.py` & `geomancy-0.8.1/tests/checks/test_env.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/tests/checks/test_exec.py` & `geomancy-0.8.1/tests/checks/test_exec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 """
 Test the CheckExec class
 """
 from geomancy.checks.exec import CheckExec
 
 
+def test_check_exec_get_current_version_no_pip():
+    """Test the CheckExec get_current_version method"""
+    check = CheckExec(name="python", value="python")
+
+    version = check.get_current_version()
+    assert isinstance(version, tuple)
+    assert version[0] >= 2  # python 2 or later
+
+
 def test_check_exec_exists():
     """Tests CheckExec checking for an existing and a missing command"""
     # Should exist
     check = CheckExec(name="Check Python", value="python3")
     assert check.check().passed
 
     # Should not exist
```

### Comparing `geomancy-0.6.3b0/tests/checks/test_path.py` & `geomancy-0.8.1/tests/checks/test_path.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/tests/checks/test_utils.py` & `geomancy-0.8.1/tests/checks/test_utils.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/tests/config/test_config.py` & `geomancy-0.8.1/tests/config/test_config.py`

 * *Files identical despite different names*

### Comparing `geomancy-0.6.3b0/tests/test_main.py` & `geomancy-0.8.1/tests/test_main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """Test the main CLI entrypoint"""
 import typing as t
+from pathlib import Path
+import os
 
 import pytest
 
 from geomancy.main import main_cli
 from geomancy.config import Config
 
 
@@ -47,15 +49,43 @@
 @pytest.mark.parametrize("options", ("--config",))
 def test_cli_config(run, options):
     """Test the --config option"""
     captured = run(options)
     assert "[config]" in captured.out  # config output in TOML format
 
 
+@pytest.mark.parametrize("flag", ("-e", "--env"))
+def test_cli_env(run, flag, test_env_file):
+    """Test the -e/--env and --overwrite flags for loading environment
+    variables.
+
+    See ./conftest.py for details on the 'test_env_file' fixture
+    """
+    # running '--overwrite' without '-e/--env' gives an error
+    captured = run("--overwrite", expected_code=2)
+
+    with pytest.MonkeyPatch.context() as mp:
+        filepath = test_env_file["filepath"]
+        variables = test_env_file["variables"]
+
+        # Reset env variables
+        for name in variables.keys():
+            mp.delenv(name, raising=False)
+
+        # running "-e/--env" should load environment variables, which are logged
+        # in debug mode
+        options = ("-d", flag, filepath)
+        captured = run(options)
+
+        # The variables are loaded in the current process
+        for name, value in variables.items():
+            assert os.environ[name] == value
+
+
 @pytest.mark.parametrize(
-    "options", ("examples/geomancy.toml", "examples/pyproject.toml")
+    "options", (Path("examples") / "geomancy.toml", Path("examples") / "pyproject.toml")
 )
 def test_cli_check(run, options):
     """Test the default checks"""
-    captured = run(options)
+    captured = run(str(options))
     # Check environment variables
     assert "Check environment variable" in captured.out
```

