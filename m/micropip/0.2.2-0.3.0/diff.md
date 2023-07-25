# Comparing `tmp/micropip-0.2.2.tar.gz` & `tmp/micropip-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropip-0.2.2.tar", last modified: Sat Mar  4 12:58:14 2023, max compression
+gzip compressed data, was "micropip-0.3.0.tar", last modified: Wed Mar 29 11:43:58 2023, max compression
```

## Comparing `micropip-0.2.2.tar` & `micropip-0.3.0.tar`

### file list

```diff
@@ -1,63 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.273306 micropip-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/.github/
--rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-04 12:57:46.000000 micropip-0.2.2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-04 12:57:46.000000 micropip-0.2.2/.github/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-03-04 12:57:46.000000 micropip-0.2.2/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-04 12:57:46.000000 micropip-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-03-04 12:57:46.000000 micropip-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      217 2023-03-04 12:57:46.000000 micropip-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (122)     2029 2023-03-04 12:57:46.000000 micropip-0.2.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-03-04 12:57:46.000000 micropip-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-03-04 12:58:14.273306 micropip-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      795 2023-03-04 12:57:46.000000 micropip-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      634 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.265306 micropip-0.2.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/_static/css/pyodide.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/docs/_static/img/
--rw-r--r--   0 runner    (1001) docker     (122)     7802 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/_static/img/pyodide-logo.png
--rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      727 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      765 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/docs/project/
--rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/project/api.md
--rw-r--r--   0 runner    (1001) docker     (122)      597 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/project/micropip-in-other-projects.md
--rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/project/usage.md
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-03-04 12:57:46.000000 micropip-0.2.2/docs/requirements-doc.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip/
--rw-r--r--   0 runner    (1001) docker     (122)      385 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/_compat.py
--rw-r--r--   0 runner    (1001) docker     (122)     1376 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/_compat_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/_compat_not_in_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (122)    30787 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/_micropip.py
--rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/_mock_package.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip/externals/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip/externals/pip/
--rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip/externals/pip/_internal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip/externals/pip/_internal/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_internal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_internal/utils/pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_internal/utils/wheel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.273306 micropip-0.2.2/micropip/externals/pip/_vendor/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_vendor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/externals/pip/_vendor/pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-03-04 12:57:46.000000 micropip-0.2.2/micropip/package.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.269306 micropip-0.2.2/micropip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1199 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-04 12:58:14.000000 micropip-0.2.2/micropip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-03-04 12:57:46.000000 micropip-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-04 12:58:14.273306 micropip-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.273306 micropip-0.2.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-04 12:58:14.273306 micropip-0.2.2/tests/dist/
--rw-r--r--   0 runner    (1001) docker     (122)    97007 2023-03-04 12:57:46.000000 micropip-0.2.2/tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (122)    36604 2023-03-04 12:57:46.000000 micropip-0.2.2/tests/test_micropip.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-03-29 11:43:34.000000 micropip-0.3.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      100 2023-03-29 11:43:34.000000 micropip-0.3.0/.github/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)     2162 2023-03-29 11:43:34.000000 micropip-0.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (122)       82 2023-03-29 11:43:34.000000 micropip-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1102 2023-03-29 11:43:34.000000 micropip-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-03-29 11:43:34.000000 micropip-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2155 2023-03-29 11:43:34.000000 micropip-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (122)    16725 2023-03-29 11:43:34.000000 micropip-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-03-29 11:43:58.967660 micropip-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-03-29 11:43:34.000000 micropip-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.959660 micropip-0.3.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      835 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/_static/css/pyodide.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/docs/_static/img/
+-rw-r--r--   0 runner    (1001) docker     (122)     7802 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/_static/img/pyodide-logo.png
+-rw-r--r--   0 runner    (1001) docker     (122)     1346 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      727 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      765 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/docs/project/
+-rw-r--r--   0 runner    (1001) docker     (122)      118 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/project/api.md
+-rw-r--r--   0 runner    (1001) docker     (122)      597 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/project/micropip-in-other-projects.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2791 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/project/usage.md
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-03-29 11:43:34.000000 micropip-0.3.0/docs/requirements-doc.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/
+-rw-r--r--   0 runner    (1001) docker     (122)      435 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      834 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1376 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_compat_in_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2741 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_compat_not_in_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30512 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_micropip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2986 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_mock_package.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/externals/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/externals/pip/
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/externals/pip/_internal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/externals/pip/_internal/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_internal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1105 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_internal/utils/pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_internal/utils/wheel.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip/externals/pip/_vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_vendor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15814 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/externals/pip/_vendor/pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2182 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/package.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3004 2023-03-29 11:43:34.000000 micropip-0.3.0/micropip/uninstall.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.963660 micropip-0.3.0/micropip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    21061 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1700 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-03-29 11:43:58.000000 micropip-0.3.0/micropip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-03-29 11:43:34.000000 micropip-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-29 11:43:58.967660 micropip-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     1851 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)    97007 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.959660 micropip-0.3.0/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/data/
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/data/data.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/deep/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/deep/deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      386 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/shallow/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/shallow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:58.967660 micropip-0.3.0/tests/test_data/test_wheel_uninstall/test_wheel_uninstall/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/test_wheel_uninstall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_data/test_wheel_uninstall/top_level.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35165 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_micropip.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6534 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_uninstall.py
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-03-29 11:43:34.000000 micropip-0.3.0/tests/test_utils.py
```

### Comparing `micropip-0.2.2/.github/workflows/main.yml` & `micropip-0.3.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/.pre-commit-config.yaml` & `micropip-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/CHANGELOG.md` & `micropip-0.3.0/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
-## Unreleased
+## [0.3.0] - 2023/03/29
+
+### Added
+
+- Added `micropip.uninstall` to uninstall packages
+  [#55](https://github.com/pyodide/micropip/pull/55)
 
 ## [0.2.2] - 2023/03/04
 
 ### Fixed
 
 - When there is an invalid version on PyPi (defined as unparsable
   by [`packaging.version.Version`](https://packaging.pypa.io/en/stable/version.html))
```

### Comparing `micropip-0.2.2/LICENSE` & `micropip-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/PKG-INFO` & `micropip-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropip
-Version: 0.2.2
+Version: 0.3.0
 Summary: A lightweight Python package installer for the web 
 Author: Pyodide developers
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `micropip-0.2.2/README.md` & `micropip-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/Makefile` & `micropip-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/_static/css/pyodide.css` & `micropip-0.3.0/docs/_static/css/pyodide.css`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/_static/img/pyodide-logo.png` & `micropip-0.3.0/docs/_static/img/pyodide-logo.png`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/conf.py` & `micropip-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/index.rst` & `micropip-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/make.bat` & `micropip-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/project/micropip-in-other-projects.md` & `micropip-0.3.0/docs/project/micropip-in-other-projects.md`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/docs/project/usage.md` & `micropip-0.3.0/docs/project/usage.md`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/_compat.py` & `micropip-0.3.0/micropip/_compat.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/_compat_in_pyodide.py` & `micropip-0.3.0/micropip/_compat_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/_compat_not_in_pyodide.py` & `micropip-0.3.0/micropip/_compat_not_in_pyodide.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/_micropip.py` & `micropip-0.3.0/micropip/_micropip.py`

 * *Files 3% similar despite different names*

```diff
@@ -688,20 +688,16 @@
         name = dist.name
         version = dist.version
         source = dist.read_text("PYODIDE_SOURCE")
         if source is None:
             # source is None if PYODIDE_SOURCE does not exist. In this case the
             # wheel was installed manually, not via `pyodide.loadPackage` or
             # `micropip`.
-            #
-            # tzdata is a funny special case: we install it with pip and then
-            # vendor it into our standard library. We should probably remove
-            # tzdata's dist-info because it's kind of weird to have dist-info in
-            # the stdlib.
             continue
+
         packages[name] = PackageMetadata(
             name=name,
             version=version,
             source=source,
         )
 
     for name, pkg_source in loadedPackages.to_py().items():
```

### Comparing `micropip-0.2.2/micropip/_mock_package.py` & `micropip-0.3.0/micropip/_mock_package.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/externals/pip/_internal/utils/pkg_resources.py` & `micropip-0.3.0/micropip/externals/pip/_internal/utils/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/externals/pip/_internal/utils/wheel.py` & `micropip-0.3.0/micropip/externals/pip/_internal/utils/wheel.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/externals/pip/_vendor/pkg_resources.py` & `micropip-0.3.0/micropip/externals/pip/_vendor/pkg_resources.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip/package.py` & `micropip-0.3.0/micropip/package.py`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/micropip.egg-info/PKG-INFO` & `micropip-0.3.0/micropip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropip
-Version: 0.2.2
+Version: 0.3.0
 Summary: A lightweight Python package installer for the web 
 Author: Pyodide developers
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
```

### Comparing `micropip-0.2.2/micropip.egg-info/SOURCES.txt` & `micropip-0.3.0/micropip.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -21,24 +21,36 @@
 docs/project/usage.md
 micropip/__init__.py
 micropip/_compat.py
 micropip/_compat_in_pyodide.py
 micropip/_compat_not_in_pyodide.py
 micropip/_micropip.py
 micropip/_mock_package.py
+micropip/_utils.py
 micropip/_version.py
 micropip/package.py
+micropip/uninstall.py
 micropip.egg-info/PKG-INFO
 micropip.egg-info/SOURCES.txt
 micropip.egg-info/dependency_links.txt
 micropip.egg-info/requires.txt
 micropip.egg-info/top_level.txt
 micropip/externals/__init__.py
 micropip/externals/pip/__init__.py
 micropip/externals/pip/_internal/__init__.py
 micropip/externals/pip/_internal/utils/__init__.py
 micropip/externals/pip/_internal/utils/pkg_resources.py
 micropip/externals/pip/_internal/utils/wheel.py
 micropip/externals/pip/_vendor/__init__.py
 micropip/externals/pip/_vendor/pkg_resources.py
+tests/conftest.py
 tests/test_micropip.py
-tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl
+tests/test_uninstall.py
+tests/test_utils.py
+tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl
+tests/test_data/test_wheel_uninstall/pyproject.toml
+tests/test_data/test_wheel_uninstall/top_level.py
+tests/test_data/test_wheel_uninstall/deep/__init__.py
+tests/test_data/test_wheel_uninstall/deep/data/data.txt
+tests/test_data/test_wheel_uninstall/deep/deep/__init__.py
+tests/test_data/test_wheel_uninstall/shallow/__init__.py
+tests/test_data/test_wheel_uninstall/test_wheel_uninstall/__init__.py
```

### Comparing `micropip-0.2.2/pyproject.toml` & `micropip-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl` & `micropip-0.3.0/tests/dist/snowballstemmer-2.0.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `micropip-0.2.2/tests/test_micropip.py` & `micropip-0.3.0/tests/test_micropip.py`

 * *Files 6% similar despite different names*

```diff
@@ -191,71 +191,26 @@
 
     result = mock_fetch_cls()
     monkeypatch.setattr(_micropip, "_get_pypi_json", result._get_pypi_json)
     monkeypatch.setattr(_micropip, "fetch_bytes", result._fetch_bytes)
     return result
 
 
-@pytest.fixture(scope="module")
-def wheel_path(tmp_path_factory):
-    # Build a micropip wheel for testing
-    import build
-    from build.env import IsolatedEnvBuilder
-
-    output_dir = tmp_path_factory.mktemp("wheel")
-
-    with IsolatedEnvBuilder() as env:
-        builder = build.ProjectBuilder(Path(__file__).parent.parent)
-        builder.python_executable = env.executable
-        builder.scripts_dir = env.scripts_dir
-        env.install(builder.build_system_requires)
-        builder.build("wheel", output_directory=output_dir)
-
-    yield output_dir
-
-
-@pytest.fixture
-def selenium_standalone_micropip(selenium_standalone, wheel_path):
-    """Import micropip before entering test so that global initialization of
-    micropip doesn't count towards hiwire refcount.
-    """
-
-    wheel_dir = Path(wheel_path)
-    wheel_files = list(wheel_dir.glob("*.whl"))
-
-    if not wheel_files:
-        pytest.exit("No wheel files found in wheel/ directory")
-
-    wheel_file = wheel_files[0]
-    with spawn_web_server(wheel_dir) as server:
-        server_hostname, server_port, _ = server
-        base_url = f"http://{server_hostname}:{server_port}/"
-        selenium_standalone.run_js(
-            f"""
-            await pyodide.loadPackage("{base_url + wheel_file.name}");
-            await pyodide.loadPackage(["packaging", "pyparsing"]);
-            pyodide.runPython("import micropip");
-            """
-        )
-
-    yield selenium_standalone
-
-
 SNOWBALL_WHEEL = "snowballstemmer-2.0.0-py2.py3-none-any.whl"
 
 
 def test_install_simple(selenium_standalone_micropip):
     selenium = selenium_standalone_micropip
     assert (
         selenium.run_js(
             """
             return await pyodide.runPythonAsync(`
                 import os
                 import micropip
-                from pyodide import to_js
+                from pyodide.ffi import to_js
                 # Package 'pyodide-micropip-test' has dependency on 'snowballstemmer'
                 # It is used to test markers support
                 await micropip.install('pyodide-micropip-test')
                 import snowballstemmer
                 stemmer = snowballstemmer.stemmer('english')
                 to_js(stemmer.stemWords('go going goes gone'.split()))
             `);
```

