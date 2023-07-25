# Comparing `tmp/ambient_package_update-23.7.1.tar.gz` & `tmp/ambient_package_update-23.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_package_update-23.7.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_package_update-23.7.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_package_update-23.7.1.tar` & `ambient_package_update-23.7.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.7.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/.gitignore
--rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1462 2023-07-25 08:05:08.152906 ambient_package_update-23.7.1/CHANGES.md
--rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/LICENSE.md
--rw-r--r--   0        0        0     4457 2023-07-25 08:05:08.168549 ambient_package_update-23.7.1/README.md
--rw-r--r--   0        0        0       93 2023-07-25 07:56:30.784223 ambient_package_update-23.7.1/ambient_package_update/__init__.py
--rw-r--r--   0        0        0     3773 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/cli.py
--rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/__init__.py
--rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/author.py
--rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient_package_update-23.7.1/ambient_package_update/metadata/constants.py
--rw-r--r--   0        0        0      592 2023-05-10 08:37:32.317360 ambient_package_update-23.7.1/ambient_package_update/metadata/package.py
--rw-r--r--   0        0        0      192 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/metadata/readme.py
--rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/ambient_package_update/metadata/ruff_ignored_inspection.py
--rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.coveragerc.tpl
--rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.editorconfig.tpl
--rw-r--r--   0        0        0     1784 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl
--rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl
--rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/.readthedocs.yml.tpl
--rw-r--r--   0        0        0     1121 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/LICENSE.md.tpl
--rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/MANIFEST.in.tpl
--rw-r--r--   0        0        0     5231 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/README.md.tpl
--rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/Makefile.tpl
--rw-r--r--   0        0        0     2847 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/conf.py.tpl
--rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/docs/make.bat.tpl
--rw-r--r--   0        0        0     3808 2023-07-25 07:54:21.598162 ambient_package_update-23.7.1/ambient_package_update/templates/pyproject.toml.tpl
--rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.7.1/ambient_package_update/templates/pytest.init.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/scripts/publish_to_pypi.ps1.tpl
--rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/scripts/publish_to_pypi.sh.tpl
--rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.7.1/ambient_package_update/templates/setup.cfg.tpl
--rw-r--r--   0        0        0     2549 2023-07-25 08:59:34.407282 ambient_package_update-23.7.1/pyproject.toml
--rw-r--r--   0        0        0     1740 2023-07-25 08:59:49.665764 ambient_package_update-23.7.1/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.1/scripts/unix/publish_to_pypi.sh
--rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.7.1/scripts/unix/setup_venv_unix.sh
--rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.1/scripts/windows/publish_to_pypi.ps1
--rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.7.1/scripts/windows/setup_venv.ps1
--rw-r--r--   0        0        0     5605 1970-01-01 00:00:00.000000 ambient_package_update-23.7.1/PKG-INFO
+-rw-r--r--   0        0        0      454 2023-05-03 13:01:37.320646 ambient_package_update-23.7.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3288 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/.gitignore
+-rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1530 2023-07-25 12:59:12.628224 ambient_package_update-23.7.2/CHANGES.md
+-rw-r--r--   0        0        0     1085 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/LICENSE.md
+-rw-r--r--   0        0        0     4457 2023-07-25 08:05:08.168549 ambient_package_update-23.7.2/README.md
+-rw-r--r--   0        0        0       93 2023-07-25 12:59:12.628224 ambient_package_update-23.7.2/ambient_package_update/__init__.py
+-rw-r--r--   0        0        0     3773 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/cli.py
+-rw-r--r--   0        0        0        0 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/ambient_package_update/metadata/__init__.py
+-rw-r--r--   0        0        0      101 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/ambient_package_update/metadata/author.py
+-rw-r--r--   0        0        0      454 2023-05-09 16:06:49.855781 ambient_package_update-23.7.2/ambient_package_update/metadata/constants.py
+-rw-r--r--   0        0        0      592 2023-05-10 08:37:32.317360 ambient_package_update-23.7.2/ambient_package_update/metadata/package.py
+-rw-r--r--   0        0        0      192 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/metadata/readme.py
+-rw-r--r--   0        0        0      110 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/ambient_package_update/metadata/ruff_ignored_inspection.py
+-rw-r--r--   0        0        0       82 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/.coveragerc.tpl
+-rw-r--r--   0        0        0      288 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/.editorconfig.tpl
+-rw-r--r--   0        0        0     1784 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/.github/workflows/ci.yml.tpl
+-rw-r--r--   0        0        0      904 2023-07-25 07:49:48.645779 ambient_package_update-23.7.2/ambient_package_update/templates/.pre-commit-config.yaml.tpl
+-rw-r--r--   0        0        0      551 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/.readthedocs.yml.tpl
+-rw-r--r--   0        0        0     1121 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/LICENSE.md.tpl
+-rw-r--r--   0        0        0      137 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/MANIFEST.in.tpl
+-rw-r--r--   0        0        0     5231 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/README.md.tpl
+-rw-r--r--   0        0        0      654 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/docs/Makefile.tpl
+-rw-r--r--   0        0        0     2847 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/docs/conf.py.tpl
+-rw-r--r--   0        0        0      795 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/docs/make.bat.tpl
+-rw-r--r--   0        0        0     3726 2023-07-25 12:26:56.740200 ambient_package_update-23.7.2/ambient_package_update/templates/pyproject.toml.tpl
+-rw-r--r--   0        0        0       56 2023-05-22 13:32:26.216194 ambient_package_update-23.7.2/ambient_package_update/templates/pytest.init.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.2/ambient_package_update/templates/scripts/publish_to_pypi.ps1.tpl
+-rw-r--r--   0        0        0       50 2023-05-22 13:32:26.231832 ambient_package_update-23.7.2/ambient_package_update/templates/scripts/publish_to_pypi.sh.tpl
+-rw-r--r--   0        0        0       69 2023-05-22 13:32:26.231832 ambient_package_update-23.7.2/ambient_package_update/templates/setup.cfg.tpl
+-rw-r--r--   0        0        0     2549 2023-07-25 08:59:34.407282 ambient_package_update-23.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1740 2023-07-25 08:59:49.665764 ambient_package_update-23.7.2/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.2/scripts/unix/publish_to_pypi.sh
+-rw-r--r--   0        0        0      566 2023-05-09 08:09:25.681131 ambient_package_update-23.7.2/scripts/unix/setup_venv_unix.sh
+-rw-r--r--   0        0        0       50 2023-05-10 08:28:40.436182 ambient_package_update-23.7.2/scripts/windows/publish_to_pypi.ps1
+-rw-r--r--   0        0        0      460 2023-05-03 13:01:37.336270 ambient_package_update-23.7.2/scripts/windows/setup_venv.ps1
+-rw-r--r--   0        0        0     5605 1970-01-01 00:00:00.000000 ambient_package_update-23.7.2/PKG-INFO
```

### Comparing `ambient_package_update-23.7.1/.gitignore` & `ambient_package_update-23.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/.pre-commit-config.yaml` & `ambient_package_update-23.7.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/CHANGES.md` & `ambient_package_update-23.7.2/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+**23.7.2 (2023-07-25)**
+* Bugfix with supported Django versions
+
 **23.7.1 (2023-07-25)**
 * Dropped Django version 2.2, 3.0, 3.1, 4.0 due to deprecation
 * Updated pre-commit linter versions
 * Updated versions for meta package
 * Added installation docs to Readme file
 
 **23.5.12 (2023-05-10)**
```

### Comparing `ambient_package_update-23.7.1/LICENSE.md` & `ambient_package_update-23.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/README.md` & `ambient_package_update-23.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/cli.py` & `ambient_package_update-23.7.2/ambient_package_update/cli.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/metadata/package.py` & `ambient_package_update-23.7.2/ambient_package_update/metadata/package.py`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/.github/workflows/ci.yml.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/.github/workflows/ci.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/.pre-commit-config.yaml.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/.pre-commit-config.yaml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/.readthedocs.yml.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/.readthedocs.yml.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/LICENSE.md.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/LICENSE.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/README.md.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/README.md.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/docs/Makefile.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/docs/Makefile.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/docs/conf.py.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/docs/conf.py.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/docs/make.bat.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/docs/make.bat.tpl`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/ambient_package_update/templates/pyproject.toml.tpl` & `ambient_package_update-23.7.2/ambient_package_update/templates/pyproject.toml.tpl`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,15 @@
     {'name' = '{{ author.name }}', 'email' = '{{ author.email }}'},{% endfor %}
 ]
 readme = "README.md"
 classifiers = [
     "Development Status :: {{ development_status }}",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -103,15 +101,15 @@
 
 # Assume Python 3.11
 target-version = "py311"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,39,310,311}-django{22,30,31,32,40,41,42}
+envlist = py{38,39,310,311}-django{32,41,42}
 isolated_build = True
 
 [testenv]
 # Django deprecation overview: https://www.djangoproject.com/download/
 deps =
     django32: Django>=3.2,<3.3
     django41: Django>=4.1,<4.2
```

### Comparing `ambient_package_update-23.7.1/pyproject.toml` & `ambient_package_update-23.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/requirements.txt` & `ambient_package_update-23.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/scripts/unix/setup_venv_unix.sh` & `ambient_package_update-23.7.2/scripts/unix/setup_venv_unix.sh`

 * *Files identical despite different names*

### Comparing `ambient_package_update-23.7.1/PKG-INFO` & `ambient_package_update-23.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-package-update
-Version: 23.7.1
+Version: 23.7.2
 Summary: Ambient package update tool for clean and swift maintenance
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

