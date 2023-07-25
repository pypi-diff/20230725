# Comparing `tmp/yapx-0.2.0.tar.gz` & `tmp/yapx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yapx-0.2.0.tar", last modified: Thu Jul 20 04:22:36 2023, max compression
+gzip compressed data, was "yapx-0.2.1.tar", last modified: Tue Jul 25 04:05:50 2023, max compression
```

## Comparing `yapx-0.2.0.tar` & `yapx-0.2.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.884490 yapx-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-07-20 04:17:57.000000 yapx-0.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5854 2023-07-20 04:22:36.884490 yapx-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4126 2023-07-20 04:17:57.000000 yapx-0.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4866 2023-07-20 04:17:57.000000 yapx-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-20 04:22:36.884490 yapx-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.876490 yapx-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.880490 yapx-0.2.0/src/yapx/
--rw-r--r--   0 root         (0) root         (0)     5155 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.880490 yapx-0.2.0/src/yapx/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     4901 2023-07-20 04:18:36.000000 yapx-0.2.0/src/yapx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-20 04:22:15.000000 yapx-0.2.0/src/yapx/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7400 2023-07-20 04:18:37.000000 yapx-0.2.0/src/yapx/__pycache__/actions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7626 2023-07-20 04:18:36.000000 yapx-0.2.0/src/yapx/__pycache__/arg.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    27582 2023-07-20 04:18:36.000000 yapx-0.2.0/src/yapx/__pycache__/argument_parser.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-20 04:18:36.000000 yapx-0.2.0/src/yapx/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      784 2023-07-20 04:18:37.000000 yapx-0.2.0/src/yapx/__pycache__/namespace.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     1550 2023-07-20 04:18:36.000000 yapx-0.2.0/src/yapx/__pycache__/types.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     4281 2023-07-20 04:18:37.000000 yapx-0.2.0/src/yapx/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-07-20 04:22:15.000000 yapx-0.2.0/src/yapx/__version__.py
--rw-r--r--   0 root         (0) root         (0)     9968 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/actions.py
--rw-r--r--   0 root         (0) root         (0)     9642 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/arg.py
--rw-r--r--   0 root         (0) root         (0)    44125 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/argument_parser.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/namespace.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/py.typed
--rw-r--r--   0 root         (0) root         (0)     1300 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/types.py
--rw-r--r--   0 root         (0) root         (0)     4214 2023-07-20 04:17:57.000000 yapx-0.2.0/src/yapx/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.880490 yapx-0.2.0/src/yapx.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5854 2023-07-20 04:22:36.000000 yapx-0.2.0/src/yapx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      981 2023-07-20 04:22:36.000000 yapx-0.2.0/src/yapx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-20 04:22:36.000000 yapx-0.2.0/src/yapx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      717 2023-07-20 04:22:36.000000 yapx-0.2.0/src/yapx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-07-20 04:22:36.000000 yapx-0.2.0/src/yapx.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-20 04:22:36.884490 yapx-0.2.0/tests/
--rw-r--r--   0 root         (0) root         (0)     5205 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_actions.py
--rw-r--r--   0 root         (0) root         (0)    11974 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_add_arguments.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_add_arguments_future.py
--rw-r--r--   0 root         (0) root         (0)     1260 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_add_command.py
--rw-r--r--   0 root         (0) root         (0)     8186 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_arg.py
--rw-r--r--   0 root         (0) root         (0)    25135 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_run.py
--rw-r--r--   0 root         (0) root         (0)     1249 2023-07-20 04:17:57.000000 yapx-0.2.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-07-25 04:01:15.000000 yapx-0.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5869 2023-07-25 04:05:50.599640 yapx-0.2.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4124 2023-07-25 04:01:15.000000 yapx-0.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     4887 2023-07-25 04:01:15.000000 yapx-0.2.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 04:05:50.599640 yapx-0.2.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.591640 yapx-0.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.595640 yapx-0.2.1/src/yapx/
+-rw-r--r--   0 root         (0) root         (0)     5155 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/src/yapx/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     4901 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-25 04:05:29.000000 yapx-0.2.1/src/yapx/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7098 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/actions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7626 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/arg.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    27701 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/argument_parser.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      921 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      784 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/namespace.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     1550 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4278 2023-07-25 04:01:56.000000 yapx-0.2.1/src/yapx/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-07-25 04:05:29.000000 yapx-0.2.1/src/yapx/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     9750 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/actions.py
+-rw-r--r--   0 root         (0) root         (0)     9642 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/arg.py
+-rw-r--r--   0 root         (0) root         (0)    44458 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/argument_parser.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/namespace.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/py.typed
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/types.py
+-rw-r--r--   0 root         (0) root         (0)     4211 2023-07-25 04:01:15.000000 yapx-0.2.1/src/yapx/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.595640 yapx-0.2.1/src/yapx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5869 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      981 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      770 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-25 04:05:50.000000 yapx-0.2.1/src/yapx.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 04:05:50.599640 yapx-0.2.1/tests/
+-rw-r--r--   0 root         (0) root         (0)     5205 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_actions.py
+-rw-r--r--   0 root         (0) root         (0)    11974 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_arguments.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_arguments_future.py
+-rw-r--r--   0 root         (0) root         (0)     1260 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_add_command.py
+-rw-r--r--   0 root         (0) root         (0)     8186 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)    25200 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)     1249 2023-07-25 04:01:15.000000 yapx-0.2.1/tests/test_utils.py
```

### Comparing `yapx-0.2.0/LICENSE` & `yapx-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/PKG-INFO` & `yapx-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Build awesome Python CLIs with ease.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://www.f2dv.com/code/r/yapx/i
 Project-URL: Repository, https://www.github.com/fresh2dev/yapx
-Project-URL: Funding, https://www.f2dv.com/funding
+Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: pydantic
 Provides-Extra: shtab
 Provides-Extra: rich
+Provides-Extra: tui
 Provides-Extra: extras
 License-File: LICENSE
 
 # yapx
 
 > Build awesome Python CLIs with ease.
 
 | Links         |                                              |
 |---------------|----------------------------------------------|
 | Code Repo     | https://www.github.com/fresh2dev/yapx        |
 | Mirror Repo   | https://www.f2dv.com/code/r/yapx             |
 | Documentation | https://www.f2dv.com/code/r/yapx/i           |
 | Changelog     | https://www.f2dv.com/code/r/yapx/i/changelog |
 | License       | https://www.f2dv.com/code/r/yapx/i/license   |
-| Funding       | https://www.f2dv.com/funding                 |
+| Funding       | https://www.f2dv.com/fund                    |
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![License](https://img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/yapx/i/license)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/pulls)
 [![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/yapx&Date)
@@ -77,16 +78,16 @@
 ```
 
 Extras are available to unlock additional functionality:
 
 - `yapx[pydantic]`: enables support for additional types
 - `yapx[shtab]`: enables shell-completion
 - `yapx[rich]`: enables prettier help and error messages
+- `yapx[tui]`: enables experimental TUI support
 - `yapx[extras]`: enables each of the above
-- `trogon-yapx`: enables experimental TUI support
 
 ## Use
 
 See notebooks of examples here:
 
 https://www.f2dv.com/code/r/yapx/i/page/overview
```

### Comparing `yapx-0.2.0/README.md` & `yapx-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 | Links         |                                              |
 |---------------|----------------------------------------------|
 | Code Repo     | https://www.github.com/fresh2dev/yapx        |
 | Mirror Repo   | https://www.f2dv.com/code/r/yapx             |
 | Documentation | https://www.f2dv.com/code/r/yapx/i           |
 | Changelog     | https://www.f2dv.com/code/r/yapx/i/changelog |
 | License       | https://www.f2dv.com/code/r/yapx/i/license   |
-| Funding       | https://www.f2dv.com/funding                 |
+| Funding       | https://www.f2dv.com/fund                    |
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![License](https://img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/yapx/i/license)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/pulls)
 [![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/yapx&Date)
@@ -49,16 +49,16 @@
 ```
 
 Extras are available to unlock additional functionality:
 
 - `yapx[pydantic]`: enables support for additional types
 - `yapx[shtab]`: enables shell-completion
 - `yapx[rich]`: enables prettier help and error messages
+- `yapx[tui]`: enables experimental TUI support
 - `yapx[extras]`: enables each of the above
-- `trogon-yapx`: enables experimental TUI support
 
 ## Use
 
 See notebooks of examples here:
 
 https://www.f2dv.com/code/r/yapx/i/page/overview
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
 # yapx > Build awesome Python CLIs with ease. | Links | | |---------------|----
 ------------------------------------------| | Code Repo | https://
 www.github.com/fresh2dev/yapx | | Mirror Repo | https://www.f2dv.com/code/r/
 yapx | | Documentation | https://www.f2dv.com/code/r/yapx/i | | Changelog |
 https://www.f2dv.com/code/r/yapx/i/changelog | | License | https://
-www.f2dv.com/code/r/yapx/i/license | | Funding | https://www.f2dv.com/funding |
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/
+www.f2dv.com/code/r/yapx/i/license | | Funding | https://www.f2dv.com/fund | [!
+[GitHub release (latest SemVer)](https://img.shields.io/github/v/release/
 fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/
 fresh2dev/yapx/releases) [![GitHub Release Date](https://img.shields.io/github/
 release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
 www.github.com/fresh2dev/yapx/releases) [![License](https://img.shields.io/
 github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
 www.f2dv.com/code/r/yapx/i/license) [![GitHub issues](https://img.shields.io/
 github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://
@@ -39,15 +39,15 @@
 booleans: `--flag` / `--no-flag` - Support for feature flags: `--dev` / `--
 test` / `--prod` - Support for counting parameters: `-vvv` - Automatic
 "helpful" arguments: `--help`, `--help-all`, `--version`, etc. - Support for
 setting values from environment variables ## Install Yapx has no 3rd-party
 dependencies out-of-the-box: ```sh pip install yapx ``` Extras are available to
 unlock additional functionality: - `yapx[pydantic]`: enables support for
 additional types - `yapx[shtab]`: enables shell-completion - `yapx[rich]`:
-enables prettier help and error messages - `yapx[extras]`: enables each of the
-above - `trogon-yapx`: enables experimental TUI support ## Use See notebooks of
+enables prettier help and error messages - `yapx[tui]`: enables experimental
+TUI support - `yapx[extras]`: enables each of the above ## Use See notebooks of
 examples here: https://www.f2dv.com/code/r/yapx/i/page/overview Read more about
 yapx @ https://www.f2dv.com/code/r/yapx/i ## Support If this project delivers
 value to you, please [provide feedback](https://www.github.com/fresh2dev/yapx/
 issues), code contributions, and/or [funding](https://www.f2dv.com/fund). See
 all of my projects @ https://www.f2dv.com/code/r *Brought to you by...* [https:
 //img.fresh2.dev/fresh2dev.svg]
```

### Comparing `yapx-0.2.0/pyproject.toml` & `yapx-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,39 +49,40 @@
     "pytest-html==3.*",
     "pytest-sugar==0.*",
     "pytest-custom-exit-code==0.3.*",
     "pylint==2.*",
     "pylint-pytest==1.*",
     "packaging==23.*",
     "pydantic>=1.10.3,<3",
-    "shtab==1.6.2",
+    "shtab==1.6.*",
     "rich-argparse==1.*",
 ]
 pydantic = [
     "pydantic>=1.10.3,<3",
 ]
 shtab = [
-    "shtab==1.6.2",
+    "shtab==1.6.*",
 ]
 rich = [
     "rich-argparse==1.*",
 ]
+tui = [
+    "argparse-tui>=0.1.2,<1",
+]
 extras = [
     "pydantic>=1.10.3,<3",
     "shtab==1.6.2",
     "rich-argparse==1.*",
+    "argparse-tui>=0.1.2,<1",
 ]
-# tui = [
-#     "trogon-argparse==0.5.0",
-# ]
 
 [project.urls]
 Homepage = "https://www.f2dv.com/code/r/yapx/i"
 Repository = "https://www.github.com/fresh2dev/yapx"
-Funding = "https://www.f2dv.com/funding"
+Funding = "https://www.f2dv.com/fund"
 
 [tool.setuptools.package-data]
 "*" = ["**"]
 [tool.setuptools.packages.find]
 where = ["src"]
 include = ["*"]
 exclude = []
```

### Comparing `yapx-0.2.0/src/yapx/__init__.py` & `yapx-0.2.1/src/yapx/__init__.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/src/yapx/__pycache__/__init__.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/__init__.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 5155 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 2314 0000  o.......u..d#...
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 2314 0000  o........I.d#...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 000f 0000 0040 0000 0073 1402 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 6d06 5a06  m.Z.m.Z.m.Z.m.Z.
 00000050: 6d07 5a07 6d08 5a08 0100 6403 6404 6c09  m.Z.m.Z...d.d.l.
 00000060: 6d0a 5a0a 6d0b 5a0b 0100 6403 6405 6c0c  m.Z.m.Z...d.d.l.
 00000070: 6d0c 5a0c 0100 6403 6406 6c0d 6d0d 5a0d  m.Z...d.d.l.m.Z.
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/arg.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/arg.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 9642 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 aa25 0000  o.......u..d.%..
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 aa25 0000  o........I.d.%..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0019 0000 0040 0000 0073 3c02 0000 5500  .....@...s<...U.
 00000030: 6400 6401 6c00 5a00 6400 6401 6c01 5a01  d.d.l.Z.d.d.l.Z.
 00000040: 6400 6402 6c02 6d03 5a03 0100 6400 6403  d.d.l.m.Z...d.d.
 00000050: 6c04 6d05 5a05 0100 6400 6404 6c06 6d07  l.m.Z...d.d.l.m.
 00000060: 5a07 6d08 5a08 6d09 5a09 6d0a 5a0a 6d0b  Z.m.Z.m.Z.m.Z.m.
 00000070: 5a0b 0100 6400 6405 6c0c 6d0d 5a0d 6d0e  Z...d.d.l.m.Z.m.
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/argument_parser.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/argument_parser.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 44125 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 5dac 0000  o.......u..d]...
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 aaad 0000  o........I.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 c401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c03 5a03 6400 6402 6c02 6d04 5a04  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 6d0a 5a0a  d.l.m.Z.m.Z.m.Z.
 00000070: 0100 6400 6405 6c0b 6d0c 5a0c 0100 6400  ..d.d.l.m.Z...d.
@@ -193,1532 +193,1540 @@
 00000c00: 726d 6174 7465 725f 636c 6173 73da 0d5f  rmatter_class.._
 00000c10: 6973 5f73 7562 7061 7273 6572 da04 6172  is_subparser..ar
 00000c20: 6773 7247 0000 0072 4800 0000 7249 0000  gsrG...rH...rI..
 00000c30: 0072 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
 00000c40: 724d 0000 0072 4e00 0000 724f 0000 00da  rM...rN...rO....
 00000c50: 066b 7761 7267 7363 0100 0000 0000 0000  .kwargsc........
 00000c60: 0900 0000 0d00 0000 0800 0000 0f00 0000  ................
-00000c70: 73e0 0100 0074 0083 006a 017c 0a7c 017c  s....t...j.|.|.|
+00000c70: 73ee 0100 0074 0083 006a 017c 0a7c 017c  s....t...j.|.|.|
 00000c80: 0972 0964 006e 017c 0364 017c 0864 029c  .r.d.n.|.d.|.d..
-00000c90: 047c 0ba4 018e 0101 0064 037c 006a 025f  .|.......d.|.j._
-00000ca0: 037c 0464 0075 0072 1e64 0464 0567 027d  .|.d.u.r.d.d.g.}
-00000cb0: 047c 0472 3674 047c 0474 0583 0272 287c  .|.r6t.|.t...r(|
-00000cc0: 0467 017d 047c 006a 0664 0664 0784 007c  .g.}.|.j.d.d...|
-00000cd0: 0444 0083 0174 0764 0864 099c 028e 0101  .D...t.d.d......
-00000ce0: 0064 0a7c 005f 0874 0964 0b64 0c84 0083  .d.|._.t.d.d....
-00000cf0: 017c 005f 0a69 007c 005f 0b7c 0973 ea7c  .|._.i.|._.|.s.|
-00000d00: 0472 5764 0d64 0784 007c 0444 0083 017d  .rWd.d...|.D...}
-00000d10: 0c7c 006a 067c 0c74 0c64 0e64 099c 028e  .|.j.|.t.d.d....
-00000d20: 0101 007c 0564 0075 0072 5e64 0f67 017d  ...|.d.u.r^d.g.}
-00000d30: 057c 0572 9674 047c 0574 0583 0272 687c  .|.r.t.|.t...rh|
-00000d40: 0567 017d 057c 006a 0d72 877c 0273 8774  .g.}.|.j.r.|.s.t
-00000d50: 0e74 0f83 018f 0e01 0074 107c 006a 0d83  .t.......t.|.j..
-00000d60: 016a 117d 0257 0064 0004 0004 0083 0301  .j.}.W.d........
-00000d70: 006e 0831 0073 8277 0101 0001 0001 0059  .n.1.s.w.......Y
-00000d80: 0001 007c 0272 967c 006a 067c 0564 1064  ...|.r.|.j.|.d.d
-00000d90: 117c 029b 009d 0264 1264 139c 038e 0101  .|.....d.d......
-00000da0: 007c 0764 0075 0072 9d64 1467 017d 0774  .|.d.u.r.d.g.}.t
-00000db0: 1272 b67c 0772 b674 047c 0774 0583 0272  .r.|.r.t.|.t...r
-00000dc0: a97c 0767 017d 077c 006a 067c 0774 1383  .|.g.}.|.j.|.t..
-00000dd0: 0074 146a 1574 1664 1564 169c 048e 0101  .t.j.t.d.d......
-00000de0: 007c 0664 0075 0072 bd64 1767 017d 067c  .|.d.u.r.d.g.}.|
-00000df0: 0672 ec74 1772 ee74 047c 0674 0583 0272  .r.t.r.t.|.t...r
-00000e00: c97c 0667 017d 0674 187c 0683 0164 186b  .|.g.}.t.|...d.k
-00000e10: 0272 e17c 0664 1919 00a0 1964 1aa1 0173  .r.|.d.....d...s
-00000e20: e174 1a7c 007c 0664 1919 0064 1b64 1c8d  .t.|.|.d...d.d..
-00000e30: 0301 0064 0053 0074 1b7c 007c 0664 1b64  ...d.S.t.|.|.d.d
-00000e40: 1c8d 0301 0064 0053 0064 0053 0064 0053  .....d.S.d.S.d.S
-00000e50: 0064 0053 0029 1d4e 4629 0472 4700 0000  .d.S.).NF).rG...
-00000e60: 7249 0000 00da 0861 6464 5f68 656c 7072  rI.....add_helpr
-00000e70: 4e00 0000 7a12 6865 6c70 6675 6c20 7061  N...z.helpful pa
-00000e80: 7261 6d65 7465 7273 7a02 2d68 7a06 2d2d  rametersz.-hz.--
-00000e90: 6865 6c70 6301 0000 0000 0000 0000 0000  helpc...........
-00000ea0: 0002 0000 0003 0000 0053 0000 0073 1400  .........S...s..
-00000eb0: 0000 6700 7c00 5d06 7d01 7c01 7202 7c01  ..g.|.].}.|.r.|.
-00000ec0: 9102 7102 5300 a900 7253 0000 00a9 02da  ..q.S...rS......
-00000ed0: 022e 30da 0178 7253 0000 0072 5300 0000  ..0..xrS...rS...
-00000ee0: fa26 2f64 726f 6e65 2f73 7263 2f73 7263  .&/drone/src/src
-00000ef0: 2f79 6170 782f 6172 6775 6d65 6e74 5f70  /yapx/argument_p
-00000f00: 6172 7365 722e 7079 da0a 3c6c 6973 7463  arser.py..<listc
-00000f10: 6f6d 703e 7400 0000 7302 0000 0014 007a  omp>t...s......z
-00000f20: 2b41 7267 756d 656e 7450 6172 7365 722e  +ArgumentParser.
-00000f30: 5f5f 696e 6974 5f5f 2e3c 6c6f 6361 6c73  __init__.<locals
-00000f40: 3e2e 3c6c 6973 7463 6f6d 703e 7a17 5368  >.<listcomp>z.Sh
-00000f50: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
-00000f60: 7361 6765 2e29 02da 0661 6374 696f 6eda  sage.)...action.
-00000f70: 0468 656c 70fa 013d 6300 0000 0000 0000  .help..=c.......
-00000f80: 0000 0000 0000 0000 0002 0000 0053 0000  .............S..
-00000f90: 0073 0800 0000 7400 7401 8301 5300 a901  .s....t.t...S...
-00000fa0: 4e29 0272 0200 0000 da04 6c69 7374 7253  N).r......listrS
-00000fb0: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
-00000fc0: 0000 da08 3c6c 616d 6264 613e 7e00 0000  ....<lambda>~...
-00000fd0: 7302 0000 0008 007a 2941 7267 756d 656e  s......z)Argumen
-00000fe0: 7450 6172 7365 722e 5f5f 696e 6974 5f5f  tParser.__init__
-00000ff0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 616d 6264  .<locals>.<lambd
-00001000: 613e 6301 0000 0000 0000 0000 0000 0002  a>c.............
-00001010: 0000 0005 0000 0053 0000 0073 2000 0000  .......S...s ...
-00001020: 6700 7c00 5d0c 7d01 7c01 a000 6400 a101  g.|.].}.|...d...
-00001030: 7202 7c01 9b00 6401 9d02 9102 7102 5300  r.|...d.....q.S.
-00001040: 2902 7a02 2d2d 7a04 2d61 6c6c a901 da0a  ).z.--z.-all....
-00001050: 7374 6172 7473 7769 7468 7254 0000 0072  startswithrT...r
-00001060: 5300 0000 7253 0000 0072 5700 0000 7258  S...rS...rW...rX
-00001070: 0000 0084 0000 00f3 0200 0000 2000 7a1b  ............ .z.
-00001080: 5368 6f77 2068 656c 7020 666f 7220 616c  Show help for al
-00001090: 6c20 636f 6d6d 616e 6473 2e7a 092d 2d76  l commands.z.--v
-000010a0: 6572 7369 6f6e da07 7665 7273 696f 6e7a  ersion..versionz
-000010b0: 0925 2870 726f 6729 7320 7a20 5368 6f77  .%(prog)s z Show
-000010c0: 2074 6865 2070 726f 6772 616d 2076 6572   the program ver
-000010d0: 7369 6f6e 206e 756d 6265 722e 2903 7259  sion number.).rY
-000010e0: 0000 0072 6200 0000 725a 0000 007a 182d  ...rb...rZ...z.-
-000010f0: 2d70 7269 6e74 2d73 6865 6c6c 2d63 6f6d  -print-shell-com
-00001100: 706c 6574 696f 6e7a 1e50 7269 6e74 2073  pletionz.Print s
-00001110: 6865 6c6c 2063 6f6d 706c 6574 696f 6e20  hell completion 
-00001120: 7363 7269 7074 2e29 0472 5900 0000 da07  script.).rY.....
-00001130: 6465 6661 756c 74da 0763 686f 6963 6573  default..choices
-00001140: 725a 0000 007a 052d 2d74 7569 7217 0000  rZ...z.--tuir...
-00001150: 0072 0100 0000 fa01 2d7a 2253 686f 7720  .r......-z"Show 
-00001160: 5465 7874 7561 6c20 5573 6572 2049 6e74  Textual User Int
-00001170: 6572 6661 6365 2028 5455 4929 2e29 03da  erface (TUI).)..
-00001180: 0670 6172 7365 72da 0e6f 7074 696f 6e5f  .parser..option_
-00001190: 7374 7269 6e67 7372 5a00 0000 291c da05  stringsrZ...)...
-000011a0: 7375 7065 72da 085f 5f69 6e69 745f 5fda  super..__init__.
-000011b0: 0a5f 6f70 7469 6f6e 616c 73da 0574 6974  ._optionals..tit
-000011c0: 6c65 da0a 6973 696e 7374 616e 6365 da03  le..isinstance..
-000011d0: 7374 72da 0c61 6464 5f61 7267 756d 656e  str..add_argumen
-000011e0: 7472 1b00 0000 da0c 6b76 5f73 6570 6172  tr......kv_separ
-000011f0: 6174 6f72 7202 0000 00da 185f 6d75 7475  atorr......_mutu
-00001200: 616c 6c79 5f65 7863 6c75 7369 7665 5f61  ally_exclusive_a
-00001210: 7267 73da 0a5f 6465 7374 5f74 7970 6572  rgs.._dest_typer
-00001220: 1c00 0000 7247 0000 0072 0300 0000 da09  ....rG...r......
-00001230: 4578 6365 7074 696f 6e72 1600 0000 7262  Exceptionr....rb
-00001240: 0000 0072 3600 0000 7232 0000 00da 0861  ...r6...r2.....a
-00001250: 7267 7061 7273 65da 0853 5550 5052 4553  rgparse..SUPPRES
-00001260: 5372 2c00 0000 7237 0000 00da 036c 656e  Sr,...r7.....len
-00001270: 7260 0000 0072 3000 0000 722f 0000 0029  r`...r0...r/...)
-00001280: 0dda 0473 656c 6672 4700 0000 7248 0000  ...selfrG...rH..
-00001290: 0072 4900 0000 724a 0000 0072 4b00 0000  .rI...rJ...rK...
-000012a0: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
-000012b0: 4f00 0000 7250 0000 0072 5100 0000 5a0e  O...rP...rQ...Z.
-000012c0: 6865 6c70 5f61 6c6c 5f66 6c61 6773 a901  help_all_flags..
-000012d0: da09 5f5f 636c 6173 735f 5f72 5300 0000  ..__class__rS...
-000012e0: 7257 0000 0072 6900 0000 5300 0000 739c  rW...ri...S...s.
-000012f0: 0000 0006 0e02 0102 010a 0102 0102 0104  ................
-00001300: fb02 0606 fa08 0a08 0208 0104 020a 0106  ................
-00001310: 0104 010c 0102 0102 0108 fd06 060a 0504  ................
-00001320: fd06 0504 0204 010e 0104 0102 0102 0102  ................
-00001330: 0108 fd08 0606 0104 020a 0106 010a 020a  ................
-00001340: 010e 011c ff04 0304 0102 0102 0108 0102  ................
-00001350: 0108 fc08 0706 0108 020a 0106 0104 0202  ................
-00001360: 0104 0104 0102 0102 0108 fb08 0806 0108  ................
-00001370: 020a 0106 011a 0202 0102 0106 0102 010a  ................
-00001380: fd02 0602 0102 0102 010a fd04 c708 2e7a  ...............z
-00001390: 1741 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
-000013a0: 5f5f 696e 6974 5f5f da07 6d65 7373 6167  __init__..messag
-000013b0: 6563 0200 0000 0000 0000 0000 0000 0200  ec..............
-000013c0: 0000 0600 0000 4300 0000 7324 0000 007c  ......C...s$...|
-000013d0: 00a0 0074 016a 02a1 0101 007c 00a0 0364  ...t.j.....|...d
-000013e0: 0164 027c 019b 0064 039d 03a1 0201 0064  .d.|...d.......d
-000013f0: 0053 0029 044e e902 0000 007a 0765 7272  .S.).N.....z.err
-00001400: 6f72 3a20 da01 0a29 04da 0b70 7269 6e74  or: ...)...print
-00001410: 5f75 7361 6765 da03 7379 73da 0673 7464  _usage..sys..std
-00001420: 6572 72da 0465 7869 7429 0272 7600 0000  err..exit).rv...
-00001430: 7279 0000 0072 5300 0000 7253 0000 0072  ry...rS...rS...r
-00001440: 5700 0000 da05 6572 726f 72c1 0000 0073  W.....error....s
-00001450: 0400 0000 0c01 1801 7a14 4172 6775 6d65  ........z.Argume
-00001460: 6e74 5061 7273 6572 2e65 7272 6f72 da04  ntParser.error..
-00001470: 6669 6c65 da10 696e 636c 7564 655f 636f  file..include_co
-00001480: 6d6d 616e 6473 da06 7265 7475 726e 6303  mmands..returnc.
-00001490: 0000 0000 0000 0000 0000 0009 0000 0005  ................
-000014a0: 0000 0003 0000 0073 8c00 0000 6401 7d03  .......s....d.}.
-000014b0: 7c03 6402 1400 6403 1700 7d04 7400 8300  |.d...d...}.t...
-000014c0: 0100 7400 7c04 8301 0100 7400 6404 7c00  ..t.|.....t.d.|.
-000014d0: 6a01 9b00 9d02 8301 0100 7400 7c04 8301  j.........t.|...
-000014e0: 0100 7c00 6a02 7d05 7403 6a04 7c00 5f02  ..|.j.}.t.j.|._.
-000014f0: 7405 8300 a006 7c01 a101 0100 7c02 7241  t.....|.....|.rA
-00001500: 7c00 a007 a100 7d06 7c06 7241 7c06 6a08  |.....}.|.rA|.j.
-00001510: a009 a100 4400 5d0b 5c02 7d07 7d08 7c08  ....D.].\.}.}.|.
-00001520: 6a06 7c01 7c02 6405 8d02 0100 7135 7c05  j.|.|.d.....q5|.
-00001530: 7c00 5f02 6406 5300 2907 6118 0200 0050  |._.d.S.).a....P
-00001540: 7269 6e74 2043 4c49 2068 656c 702e 0a0a  rint CLI help...
-00001550: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00001560: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00001570: 655f 636f 6d6d 616e 6473 3a20 6966 2054  e_commands: if T
-00001580: 7275 652c 2061 6c73 6f20 7072 696e 7420  rue, also print 
-00001590: 6865 6c70 2066 6f72 2065 6163 6820 636f  help for each co
-000015a0: 6d6d 616e 642e 0a0a 2020 2020 2020 2020  mmand...        
-000015b0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-000015c0: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-000015d0: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
-000015e0: 2020 3e3e 3e20 6672 6f6d 2064 6174 6163    >>> from datac
-000015f0: 6c61 7373 6573 2069 6d70 6f72 7420 6461  lasses import da
-00001600: 7461 636c 6173 730a 2020 2020 2020 2020  taclass.        
-00001610: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001620: 2020 2020 3e3e 3e20 4064 6174 6163 6c61      >>> @datacla
-00001630: 7373 0a20 2020 2020 2020 2020 2020 202e  ss.            .
-00001640: 2e2e 2063 6c61 7373 2041 6464 4e75 6d73  .. class AddNums
-00001650: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00001660: 2e20 2020 2020 783a 2069 6e74 0a20 2020  .     x: int.   
-00001670: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00001680: 2079 3a20 696e 740a 2020 2020 2020 2020   y: int.        
-00001690: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-000016a0: 2020 2020 3e3e 3e20 7061 7273 6572 203d      >>> parser =
-000016b0: 2079 6170 782e 4172 6775 6d65 6e74 5061   yapx.ArgumentPa
-000016c0: 7273 6572 2829 0a20 2020 2020 2020 2020  rser().         
-000016d0: 2020 203e 3e3e 2070 6172 7365 722e 6164     >>> parser.ad
-000016e0: 645f 6172 6775 6d65 6e74 7328 4164 644e  d_arguments(AddN
-000016f0: 756d 7329 0a20 2020 2020 2020 2020 2020  ums).           
-00001700: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00001710: 203e 3e3e 2070 6172 7365 722e 7072 696e   >>> parser.prin
-00001720: 745f 6865 6c70 2869 6e63 6c75 6465 5f63  t_help(include_c
-00001730: 6f6d 6d61 6e64 733d 5472 7565 2920 2023  ommands=True)  #
-00001740: 646f 6374 6573 743a 202b 534b 4950 0a20  doctest: +SKIP. 
-00001750: 2020 2020 2020 20da 015f e950 0000 0072         .._.P...r
-00001760: 7b00 0000 7a02 2420 2901 7282 0000 004e  {...z.$ ).r....N
-00001770: 290a da05 7072 696e 7472 4700 0000 da05  )...printrG.....
-00001780: 7573 6167 6572 7300 0000 7274 0000 0072  usagers...rt...r
-00001790: 6800 0000 da0a 7072 696e 745f 6865 6c70  h.....print_help
-000017a0: da0f 5f67 6574 5f73 7562 7061 7273 6572  .._get_subparser
-000017b0: 7372 6400 0000 da05 6974 656d 7329 0972  srd.....items).r
-000017c0: 7600 0000 7281 0000 0072 8200 0000 5a08  v...r....r....Z.
-000017d0: 7365 705f 6368 6172 da09 7365 7061 7261  sep_char..separa
-000017e0: 746f 7272 8700 0000 da0a 7375 6270 6172  torr......subpar
-000017f0: 7365 7273 5a07 5f63 686f 6963 655a 0973  sersZ._choiceZ.s
-00001800: 7562 7061 7273 6572 7277 0000 0072 5300  ubparserrw...rS.
-00001810: 0000 7257 0000 0072 8800 0000 c500 0000  ..rW...r........
-00001820: 731e 0000 0004 180c 0106 0108 0110 0108  s...............
-00001830: 0106 0308 010c 0204 0208 0104 0112 0110  ................
-00001840: 010a 027a 1941 7267 756d 656e 7450 6172  ...z.ArgumentPar
-00001850: 7365 722e 7072 696e 745f 6865 6c70 da0a  ser.print_help..
-00001860: 6172 6773 5f6d 6f64 656c 2e63 0200 0000  args_model.c....
-00001870: 0000 0000 0000 0000 0200 0000 0400 0000  ................
-00001880: 4300 0000 7310 0000 007c 00a0 007c 007c  C...s....|...|.|
-00001890: 01a1 0201 0064 0153 0029 0261 d605 0000  .....d.S.).a....
-000018a0: 4164 6420 6172 6775 6d65 6e74 7320 6672  Add arguments fr
-000018b0: 6f6d 2074 6865 2067 6976 656e 2066 756e  om the given fun
-000018c0: 6374 696f 6e20 6f72 2064 6174 6166 7261  ction or datafra
-000018d0: 6d65 2e0a 0a20 2020 2020 2020 2041 7267  me...        Arg
-000018e0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-000018f0: 7267 735f 6d6f 6465 6c3a 2061 2066 756e  rgs_model: a fun
-00001900: 6374 696f 6e20 6f72 2064 6174 6163 6c61  ction or datacla
-00001910: 7373 2066 726f 6d20 7768 6963 6820 746f  ss from which to
-00001920: 2064 6572 6976 6520 6172 6775 6d65 6e74   derive argument
-00001930: 732e 0a0a 2020 2020 2020 2020 4578 616d  s...        Exam
-00001940: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
-00001950: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-00001960: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
-00001970: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
-00001980: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00001990: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-000019a0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-000019b0: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-000019c0: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
-000019d0: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
-000019e0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-000019f0: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
-00001a00: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
-00001a10: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00001a20: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00001a30: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
-00001a40: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
-00001a50: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
-00001a60: 3e3e 2070 6172 7365 722e 6164 645f 6172  >> parser.add_ar
-00001a70: 6775 6d65 6e74 7328 4164 644e 756d 7329  guments(AddNums)
-00001a80: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00001a90: 2070 6172 7365 722e 7365 745f 6465 6661   parser.set_defa
-00001aa0: 756c 7473 285f 636f 6d6d 616e 645f 6675  ults(_command_fu
-00001ab0: 6e63 3d6c 616d 6264 6120 782c 2079 3a20  nc=lambda x, y: 
-00001ac0: 782b 7929 0a20 2020 2020 2020 2020 2020  x+y).           
-00001ad0: 203e 3e3e 2070 6172 7365 6420 3d20 7061   >>> parsed = pa
-00001ae0: 7273 6572 2e70 6172 7365 5f61 7267 7328  rser.parse_args(
-00001af0: 5b27 2d78 272c 2027 3127 2c20 272d 7927  ['-x', '1', '-y'
-00001b00: 2c20 2732 275d 290a 2020 2020 2020 2020  , '2']).        
-00001b10: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-00001b20: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
-00001b30: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
-00001b40: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
-00001b50: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00001b60: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
-00001b70: 6675 6e63 5f61 7267 735f 6d6f 6465 6c28  func_args_model(
-00001b80: 783d 7061 7273 6564 2e78 2c20 793d 7061  x=parsed.x, y=pa
-00001b90: 7273 6564 2e79 290a 2020 2020 2020 2020  rsed.y).        
-00001ba0: 2020 2020 4164 644e 756d 7328 783d 312c      AddNums(x=1,
-00001bb0: 2079 3d32 290a 2020 2020 2020 2020 2020   y=2).          
-00001bc0: 2020 3e3e 3e20 7061 7273 6564 2e5f 636f    >>> parsed._co
-00001bd0: 6d6d 616e 645f 6675 6e63 2878 3d70 6172  mmand_func(x=par
-00001be0: 7365 642e 782c 2079 3d70 6172 7365 642e  sed.x, y=parsed.
-00001bf0: 7929 0a20 2020 2020 2020 2020 2020 2033  y).            3
-00001c00: 0a0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00001c10: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
-00001c20: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00001c30: 2020 2020 2020 2020 2020 3e3e 3e20 6465            >>> de
-00001c40: 6620 6164 645f 6e75 6d73 2878 3a20 696e  f add_nums(x: in
-00001c50: 742c 2079 3a20 696e 7429 3a0a 2020 2020  t, y: int):.    
-00001c60: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00001c70: 7265 7475 726e 2078 202b 2079 0a20 2020  return x + y.   
-00001c80: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
-00001c90: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
-00001ca0: 7365 7220 3d20 7961 7078 2e41 7267 756d  ser = yapx.Argum
-00001cb0: 656e 7450 6172 7365 7228 290a 2020 2020  entParser().    
-00001cc0: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
-00001cd0: 6572 2e61 6464 5f61 7267 756d 656e 7473  er.add_arguments
-00001ce0: 2861 6464 5f6e 756d 7329 0a20 2020 2020  (add_nums).     
-00001cf0: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
-00001d00: 722e 7365 745f 6465 6661 756c 7473 285f  r.set_defaults(_
-00001d10: 636f 6d6d 616e 645f 6675 6e63 3d61 6464  command_func=add
-00001d20: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
-00001d30: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
-00001d40: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
-00001d50: 7328 5b27 2d78 272c 2027 3127 2c20 272d  s(['-x', '1', '-
-00001d60: 7927 2c20 2732 275d 290a 2020 2020 2020  y', '2']).      
-00001d70: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00001d80: 2020 2020 2020 3e3e 3e20 2870 6172 7365        >>> (parse
-00001d90: 642e 782c 2070 6172 7365 642e 7929 0a20  d.x, parsed.y). 
-00001da0: 2020 2020 2020 2020 2020 2028 312c 2032             (1, 2
-00001db0: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00001dc0: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
-00001dd0: 645f 6675 6e63 5f61 7267 735f 6d6f 6465  d_func_args_mode
-00001de0: 6c28 783d 7061 7273 6564 2e78 2c20 793d  l(x=parsed.x, y=
-00001df0: 7061 7273 6564 2e79 290a 2020 2020 2020  parsed.y).      
-00001e00: 2020 2020 2020 4461 7461 636c 6173 735f        Dataclass_
-00001e10: 6164 645f 6e75 6d73 2878 3d31 2c20 793d  add_nums(x=1, y=
-00001e20: 3229 0a20 2020 2020 2020 2020 2020 203e  2).            >
-00001e30: 3e3e 2070 6172 7365 642e 5f63 6f6d 6d61  >> parsed._comma
-00001e40: 6e64 5f66 756e 6328 783d 7061 7273 6564  nd_func(x=parsed
-00001e50: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
-00001e60: 2020 2020 2020 2020 2020 2020 330a 2020              3.  
-00001e70: 2020 2020 2020 4e29 01da 0e5f 6164 645f        N)..._add_
-00001e80: 6172 6775 6d65 6e74 7329 0272 7600 0000  arguments).rv...
-00001e90: 728d 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
-00001ea0: 5700 0000 da0d 6164 645f 6172 6775 6d65  W.....add_argume
-00001eb0: 6e74 73f2 0000 0073 0200 0000 102f 7a1c  nts....s...../z.
-00001ec0: 4172 6775 6d65 6e74 5061 7273 6572 2e61  ArgumentParser.a
-00001ed0: 6464 5f61 7267 756d 656e 7473 da04 6e61  dd_arguments..na
-00001ee0: 6d65 6303 0000 0000 0000 0000 0000 0009  mec.............
-00001ef0: 0000 0005 0000 004b 0000 0073 9800 0000  .......K...s....
-00001f00: 7c00 a000 a100 7d04 7c02 730b 7401 7c01  |.....}.|.s.t.|.
-00001f10: 6a02 8301 7d02 7403 7c04 7404 6a05 8302  j...}.t.|.t.j...
-00001f20: 7313 4a00 8201 7c03 a006 6401 6402 a102  s.J...|...d.d...
-00001f30: 7d05 7c05 7221 7c05 6403 7c02 1700 3700  }.|.r!|.d.|...7.
-00001f40: 7d05 7c00 6a07 7c01 6404 8d01 7d06 6402  }.|.j.|.d...}.d.
-00001f50: 7d07 7c06 7231 7c06 a008 a100 6405 1900  }.|.r1|.....d...
-00001f60: 7d07 7c04 6a09 7c02 6601 7c05 7c07 6406  }.|.j.|.f.|.|.d.
-00001f70: 9c02 7c03 a401 8e01 7d08 7c06 7242 7c06  ..|.....}.|.rB|.
-00001f80: 7c08 5f0a 7c01 724a 7c00 a00b 7c08 7c01  |._.|.rJ|...|.|.
-00001f90: a102 0100 7c08 5300 2907 6159 0800 0043  ....|.S.).aY...C
-00001fa0: 7265 6174 6520 6120 6e65 7720 7375 6263  reate a new subc
-00001fb0: 6f6d 6d61 6e64 2061 6e64 2061 6464 2061  ommand and add a
-00001fc0: 7267 756d 656e 7473 2066 726f 6d20 7468  rguments from th
-00001fd0: 6520 6769 7665 6e20 6675 6e63 7469 6f6e  e given function
-00001fe0: 206f 7220 6461 7461 6672 616d 6520 746f   or dataframe to
-00001ff0: 2069 742e 0a0a 2020 2020 2020 2020 4172   it...        Ar
-00002000: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00002010: 6172 6773 5f6d 6f64 656c 3a20 6120 6675  args_model: a fu
-00002020: 6e63 7469 6f6e 206f 7220 6461 7461 636c  nction or datacl
-00002030: 6173 7320 6672 6f6d 2077 6869 6368 2074  ass from which t
-00002040: 6f20 6465 7269 7665 2061 7267 756d 656e  o derive argumen
-00002050: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00002060: 6e61 6d65 3a20 6e61 6d65 206f 6620 7468  name: name of th
-00002070: 6520 636f 6d6d 616e 640a 0a20 2020 2020  e command..     
-00002080: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00002090: 2020 2020 2020 2020 7468 6520 6e65 7720          the new 
-000020a0: 6172 6770 6172 7365 2073 7562 7061 7273  argparse subpars
-000020b0: 6572 0a0a 2020 2020 2020 2020 4578 616d  er..        Exam
-000020c0: 706c 6573 3a0a 2020 2020 2020 2020 2020  ples:.          
-000020d0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
-000020e0: 780a 2020 2020 2020 2020 2020 2020 3e3e  x.            >>
-000020f0: 3e20 6672 6f6d 2064 6174 6163 6c61 7373  > from dataclass
-00002100: 6573 2069 6d70 6f72 7420 6461 7461 636c  es import datacl
-00002110: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
-00002120: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00002130: 3e3e 3e20 4064 6174 6163 6c61 7373 0a20  >>> @dataclass. 
-00002140: 2020 2020 2020 2020 2020 202e 2e2e 2063             ... c
-00002150: 6c61 7373 2041 6464 4e75 6d73 3a0a 2020  lass AddNums:.  
-00002160: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00002170: 2020 783a 2069 6e74 0a20 2020 2020 2020    x: int.       
-00002180: 2020 2020 202e 2e2e 2020 2020 2079 3a20       ...     y: 
-00002190: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-000021a0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-000021b0: 3e3e 3e20 7061 7273 6572 203d 2079 6170  >>> parser = yap
-000021c0: 782e 4172 6775 6d65 6e74 5061 7273 6572  x.ArgumentParser
-000021d0: 2829 0a20 2020 2020 2020 2020 2020 203e  ().            >
-000021e0: 3e3e 2073 7562 7061 7273 6572 5f31 203d  >> subparser_1 =
-000021f0: 2070 6172 7365 722e 6164 645f 636f 6d6d   parser.add_comm
-00002200: 616e 6428 4164 644e 756d 732c 206e 616d  and(AddNums, nam
-00002210: 653d 2761 6464 2729 0a20 2020 2020 2020  e='add').       
-00002220: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
-00002230: 6572 5f31 2e73 6574 5f64 6566 6175 6c74  er_1.set_default
-00002240: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
-00002250: 6c61 6d62 6461 2078 2c20 793a 2078 2b79  lambda x, y: x+y
-00002260: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
-00002270: 3e20 7375 6270 6172 7365 725f 3220 3d20  > subparser_2 = 
-00002280: 7061 7273 6572 2e61 6464 5f63 6f6d 6d61  parser.add_comma
-00002290: 6e64 2841 6464 4e75 6d73 2c20 6e61 6d65  nd(AddNums, name
-000022a0: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
-000022b0: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
-000022c0: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
-000022d0: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
-000022e0: 756e 633d 6c61 6d62 6461 2078 2c20 793a  unc=lambda x, y:
-000022f0: 2078 2d79 290a 2020 2020 2020 2020 2020   x-y).          
-00002300: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00002310: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
-00002320: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
-00002330: 285b 2761 6464 272c 2027 2d78 272c 2027  (['add', '-x', '
-00002340: 3127 2c20 272d 7927 2c20 2732 275d 290a  1', '-y', '2']).
-00002350: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00002360: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002370: 2870 6172 7365 642e 782c 2070 6172 7365  (parsed.x, parse
-00002380: 642e 7929 0a20 2020 2020 2020 2020 2020  d.y).           
-00002390: 2028 312c 2032 290a 2020 2020 2020 2020   (1, 2).        
-000023a0: 2020 2020 3e3e 3e20 7061 7273 6564 2e5f      >>> parsed._
-000023b0: 636f 6d6d 616e 645f 6675 6e63 5f61 7267  command_func_arg
-000023c0: 735f 6d6f 6465 6c28 783d 7061 7273 6564  s_model(x=parsed
-000023d0: 2e78 2c20 793d 7061 7273 6564 2e79 290a  .x, y=parsed.y).
-000023e0: 2020 2020 2020 2020 2020 2020 4164 644e              AddN
-000023f0: 756d 7328 783d 312c 2079 3d32 290a 2020  ums(x=1, y=2).  
-00002400: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00002410: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
-00002420: 6e63 2878 3d70 6172 7365 642e 782c 2079  nc(x=parsed.x, y
-00002430: 3d70 6172 7365 642e 7929 0a20 2020 2020  =parsed.y).     
-00002440: 2020 2020 2020 2033 0a0a 2020 2020 2020         3..      
-00002450: 2020 2020 2020 3e3e 3e20 696d 706f 7274        >>> import
-00002460: 2079 6170 780a 2020 2020 2020 2020 2020   yapx.          
-00002470: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00002480: 2020 3e3e 3e20 6465 6620 6164 645f 6e75    >>> def add_nu
-00002490: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
-000024a0: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
-000024b0: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
-000024c0: 202b 2079 0a20 2020 2020 2020 2020 2020   + y.           
-000024d0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-000024e0: 203e 3e3e 2064 6566 2073 7562 7472 6163   >>> def subtrac
-000024f0: 745f 6e75 6d73 2878 3a20 696e 742c 2079  t_nums(x: int, y
-00002500: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
-00002510: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
-00002520: 726e 2078 202d 2079 0a20 2020 2020 2020  rn x - y.       
-00002530: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00002540: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
-00002550: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
-00002560: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
-00002570: 2020 2020 3e3e 3e20 7375 6270 6172 7365      >>> subparse
-00002580: 725f 3120 3d20 7061 7273 6572 2e61 6464  r_1 = parser.add
-00002590: 5f63 6f6d 6d61 6e64 2861 6464 5f6e 756d  _command(add_num
-000025a0: 732c 206e 616d 653d 2761 6464 2729 0a20  s, name='add'). 
-000025b0: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
-000025c0: 7562 7061 7273 6572 5f31 2e73 6574 5f64  ubparser_1.set_d
-000025d0: 6566 6175 6c74 7328 5f63 6f6d 6d61 6e64  efaults(_command
-000025e0: 5f66 756e 633d 6164 645f 6e75 6d73 290a  _func=add_nums).
-000025f0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00002600: 7375 6270 6172 7365 725f 3220 3d20 7061  subparser_2 = pa
-00002610: 7273 6572 2e61 6464 5f63 6f6d 6d61 6e64  rser.add_command
-00002620: 2873 7562 7472 6163 745f 6e75 6d73 2c20  (subtract_nums, 
-00002630: 6e61 6d65 3d27 7375 6274 7261 6374 2729  name='subtract')
-00002640: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00002650: 2073 7562 7061 7273 6572 5f32 2e73 6574   subparser_2.set
-00002660: 5f64 6566 6175 6c74 7328 5f63 6f6d 6d61  _defaults(_comma
-00002670: 6e64 5f66 756e 633d 7375 6274 7261 6374  nd_func=subtract
-00002680: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
-00002690: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-000026a0: 2020 203e 3e3e 2070 6172 7365 6420 3d20     >>> parsed = 
-000026b0: 7061 7273 6572 2e70 6172 7365 5f61 7267  parser.parse_arg
-000026c0: 7328 5b27 7375 6274 7261 6374 272c 2027  s(['subtract', '
-000026d0: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
-000026e0: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
-000026f0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00002700: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
-00002710: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
-00002720: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
-00002730: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00002740: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
-00002750: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
-00002760: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
-00002770: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
-00002780: 2020 4461 7461 636c 6173 735f 7375 6274    Dataclass_subt
-00002790: 7261 6374 5f6e 756d 7328 783d 312c 2079  ract_nums(x=1, y
-000027a0: 3d32 290a 2020 2020 2020 2020 2020 2020  =2).            
-000027b0: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
-000027c0: 616e 645f 6675 6e63 2878 3d70 6172 7365  and_func(x=parse
-000027d0: 642e 782c 2079 3d70 6172 7365 642e 7929  d.x, y=parsed.y)
-000027e0: 0a20 2020 2020 2020 2020 2020 202d 310a  .            -1.
-000027f0: 2020 2020 2020 2020 7247 0000 004e fa01          rG...N..
-00002800: 20a9 0172 8d00 0000 7201 0000 0029 0272   ..r....r....).r
-00002810: 4700 0000 725a 0000 0029 0cda 165f 6765  G...rZ...)..._ge
-00002820: 745f 6f72 5f61 6464 5f73 7562 7061 7273  t_or_add_subpars
-00002830: 6572 7372 2400 0000 da08 5f5f 6e61 6d65  ersr$.....__name
-00002840: 5f5f 726c 0000 0072 7300 0000 da11 5f53  __rl...rs....._S
-00002850: 7562 5061 7273 6572 7341 6374 696f 6eda  ubParsersAction.
-00002860: 0370 6f70 da1f 5f67 6574 5f64 6573 6372  .pop.._get_descr
-00002870: 6970 7469 6f6e 5f66 726f 6d5f 646f 6373  iption_from_docs
-00002880: 7472 696e 67da 0a73 706c 6974 6c69 6e65  tring..splitline
-00002890: 73da 0a61 6464 5f70 6172 7365 7272 4900  s..add_parserrI.
-000028a0: 0000 728e 0000 0029 0972 7600 0000 728d  ..r....).rv...r.
-000028b0: 0000 0072 9000 0000 7251 0000 0072 8c00  ...r....rQ...r..
-000028c0: 0000 7247 0000 005a 0f64 6573 6372 6970  ..rG...Z.descrip
-000028d0: 7469 6f6e 5f74 7874 5a08 6865 6c70 5f74  tion_txtZ.help_t
-000028e0: 7874 7266 0000 0072 5300 0000 7253 0000  xtrf...rS...rS..
-000028f0: 0072 5700 0000 da0b 6164 645f 636f 6d6d  .rW.....add_comm
-00002900: 616e 6423 0100 0073 3400 0000 083e 0402  and#...s4....>..
-00002910: 0a01 1003 0c01 0401 0c01 0404 0201 06ff  ................
-00002920: 0403 0401 0c01 0402 0201 02ff 0202 0201  ................
-00002930: 04fd 0204 06fc 0406 0601 0402 0c01 0402  ................
-00002940: 7a1a 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
-00002950: 2e61 6464 5f63 6f6d 6d61 6e64 da04 6675  .add_command..fu
-00002960: 6e63 6303 0000 0000 0000 0000 0000 0005  ncc.............
-00002970: 0000 0005 0000 004b 0000 0073 4200 0000  .......K...sB...
-00002980: 7400 7c02 7205 7c02 6e02 7c01 6a01 8301  t.|.r.|.n.|.j...
-00002990: 7d02 7c00 6a02 7c01 6601 6401 7c02 6901  }.|.j.|.f.d.|.i.
-000029a0: 7c03 a401 8e01 7d04 7c04 6a03 6402 6900  |.....}.|.j.d.i.
-000029b0: 7c00 6a04 7c01 6901 a401 8e01 0100 6400  |.j.|.i.......d.
-000029c0: 5300 2903 4e72 9000 0000 7253 0000 0029  S.).Nr....rS...)
-000029d0: 0572 2400 0000 7294 0000 0072 9a00 0000  .r$...r....r....
-000029e0: da0c 7365 745f 6465 6661 756c 7473 7245  ..set_defaultsrE
-000029f0: 0000 0029 0572 7600 0000 729b 0000 0072  ...).rv...r....r
-00002a00: 9000 0000 7251 0000 0072 6600 0000 7253  ....rQ...rf...rS
-00002a10: 0000 0072 5300 0000 7257 0000 00da 115f  ...rS...rW....._
-00002a20: 7265 6769 7374 6572 5f63 6f6d 6d61 6e64  register_command
-00002a30: 8301 0000 7312 0000 0012 0604 0102 0104  ....s...........
-00002a40: ff02 0202 fe02 0306 fd1a 057a 2041 7267  ...........z Arg
-00002a50: 756d 656e 7450 6172 7365 722e 5f72 6567  umentParser._reg
-00002a60: 6973 7465 725f 636f 6d6d 616e 64da 0464  ister_command..d
-00002a70: 636c 73da 0461 7474 7263 0200 0000 0000  cls..attrc......
-00002a80: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
-00002a90: 0000 730a 0000 007c 017c 006a 0076 0153  ..s....|.|.j.v.S
-00002aa0: 0072 5c00 0000 a901 da0f 5f5f 616e 6e6f  .r\.......__anno
-00002ab0: 7461 7469 6f6e 735f 5fa9 0272 9e00 0000  tations__..r....
-00002ac0: 729f 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
-00002ad0: 5700 0000 da17 5f69 735f 6174 7472 6962  W....._is_attrib
-00002ae0: 7574 655f 696e 6865 7269 7465 6491 0100  ute_inherited...
-00002af0: 0073 0200 0000 0a02 7a26 4172 6775 6d65  .s......z&Argume
-00002b00: 6e74 5061 7273 6572 2e5f 6973 5f61 7474  ntParser._is_att
-00002b10: 7269 6275 7465 5f69 6e68 6572 6974 6564  ribute_inherited
-00002b20: 7266 0000 0063 0300 0000 0000 0000 0000  rf...c..........
-00002b30: 0000 1900 0000 0900 0000 0300 0000 73f2  ..............s.
-00002b40: 0600 0074 007c 0283 0172 077c 0289 016e  ...t.|...r.|...n
-00002b50: 0474 017c 0283 0189 017c 01a0 0288 006a  .t.|.....|.....j
-00002b60: 03a1 0172 1864 017d 037c 01a0 047c 03a1  ...r.d.}.|...|..
-00002b70: 0101 007c 016a 0564 2269 0088 006a 0388  ...|.j.d"i...j..
-00002b80: 0169 01a4 018e 0101 0069 007d 0474 0674  .i.......i.}.t.t
-00002b90: 0787 0087 0166 0264 0264 0384 0874 0888  .....f.d.d...t..
-00002ba0: 0183 0183 0283 017d 0564 0464 0584 007c  .......}.d.d...|
-00002bb0: 0544 0083 017d 0667 007d 077c 0644 0090  .D...}.g.}.|.D..
-00002bc0: 035d 375c 027d 087d 097c 086a 097d 0a74  .]7\.}.}.|.j.}.t
-00002bd0: 0a7c 0a74 0b83 0272 4f74 0c7c 0a83 017d  .|.t...rOt.|...}
-00002be0: 0a74 0a7c 0a74 0b83 0272 564a 0082 0174  .t.|.t...rVJ...t
-00002bf0: 0d6a 0e64 066b 0572 6074 0a7c 0a74 0f83  .j.d.k.r`t.|.t..
-00002c00: 0273 6788 00a0 107c 0aa1 0174 1175 0072  .sg....|...t.u.r
-00002c10: 6e88 006a 127c 0a64 0764 088d 027d 0a74  n..j.|.d.d...}.t
-00002c20: 0a7c 0a74 1383 0272 a988 00a0 147c 0aa1  .|.t...r.....|..
-00002c30: 0144 005d 137d 0b74 157c 0b74 1683 0272  .D.].}.t.|.t...r
-00002c40: 8b74 177c 0b6a 1876 0072 8b7c 0b6a 1874  .t.|.j.v.r.|.j.t
-00002c50: 1719 007d 0901 006e 0171 7888 00a0 107c  ...}...n.qx....|
-00002c60: 0aa1 017d 0a74 0d6a 0e64 066b 0572 9b74  ...}.t.j.d.k.r.t
-00002c70: 0a7c 0a74 0f83 0273 a288 00a0 107c 0aa1  .|.t...s.....|..
-00002c80: 0174 1175 0072 a988 006a 127c 0a64 0764  .t.u.r...j.|.d.d
-00002c90: 088d 027d 0a74 0a7c 0a74 0983 0272 b17c  ...}.t.|.t...r.|
-00002ca0: 0a6a 196e 0a74 0b7c 0a83 016a 1a64 0964  .j.n.t.|...j.d.d
-00002cb0: 0a64 0b8d 0264 0c19 007d 0c7c 09a0 1b7c  .d...d...}.|...|
-00002cc0: 086a 1ca1 0101 007c 096a 1d72 df7c 086a  .j.....|.j.r.|.j
-00002cd0: 1e74 1f75 0172 d27c 086a 1e7c 095f 1e64  .t.u.r.|.j.|._.d
-00002ce0: 0d7c 095f 1d6e 0d7c 086a 2074 1f75 0172  .|._.n.|.j t.u.r
-00002cf0: df7c 08a0 20a1 007c 095f 1e64 0d7c 095f  .|.. ..|._.d.|._
-00002d00: 1d88 00a0 107c 0aa1 017d 0d7c 0d90 0172  .....|...}.|...r
-00002d10: 6f7c 0d90 0172 037c 0d74 2175 0090 0172  o|...r.|.t!u...r
-00002d20: 0374 0688 00a0 227c 0aa1 0183 017c 095f  .t...."|.....|._
-00002d30: 237c 096a 2390 0172 0274 097c 096a 2364  #|.j#..r.t.|.j#d
-00002d40: 0e19 0083 017d 0a6e 7774 247c 0d74 256a  .....}.nwt$|.t%j
-00002d50: 266a 2783 0290 0172 1a88 006a 127c 0a64  &j'....r...j.|.d
-00002d60: 0764 0f8d 027d 0a7c 096a 2890 0173 1974  .d...}.|.j(..s.t
-00002d70: 297c 095f 286e 3574 247c 0d74 256a 266a  )|._(n5t$|.t%j&j
-00002d80: 2a83 0290 0173 277c 0d74 2b75 0090 0172  *....s'|.t+u...r
-00002d90: 4888 006a 127c 0a64 0764 0f8d 027d 0a7c  H..j.|.d.d...}.|
-00002da0: 096a 2890 0173 477c 0d74 2b75 0090 0172  .j(..sG|.t+u...r
-00002db0: 3b74 2c7c 095f 286e 147c 0d74 2d75 0090  ;t,|._(n.|.t-u..
-00002dc0: 0172 4474 2e7c 095f 286e 0b74 2f7c 095f  .rDt.|._(n.t/|._
-00002dd0: 286e 0774 3090 0173 4f74 317c 0a83 0101  (n.t0..sOt1|....
-00002de0: 0074 247c 0a74 3283 0290 0172 5d64 1064  .t$|.t2....r]d.d
-00002df0: 0584 007c 0a44 0083 017c 095f 2374 157c  ...|.D...|._#t.|
-00002e00: 0188 0083 0290 0172 6c74 3374 347c 0a83  .......rlt3t4|..
-00002e10: 027c 016a 357c 096a 363c 0074 0b7d 0a6e  .|.j5|.j6<.t.}.n
-00002e20: 0b74 247c 0a74 3283 0290 0172 7a74 067c  .t$|.t2....rzt.|
-00002e30: 0a83 017c 095f 237c 0a7c 095f 097c 09a0  ...|._#|.|._.|..
-00002e40: 37a1 007d 0e7c 0e64 113d 007c 0ea0 3864  7..}.|.d.=.|..8d
-00002e50: 12a1 017d 0f7c 0f90 0173 8e67 006e 0664  ...}.|...s.g.n.d
-00002e60: 1364 0584 007c 0f44 0083 017d 107c 0e64  .d...|.D...}.|.d
-00002e70: 1419 0090 0173 b17c 0ea0 3964 15a1 0190  .....s.|..9d....
-00002e80: 0173 b17c 1090 0173 ad64 167c 0e64 1719  .s.|...s.d.|.d..
-00002e90: 00a0 3aa1 009b 0064 189d 036e 0164 197c  ..:....d...n.d.|
-00002ea0: 0e64 143c 007c 0e64 1a19 007d 117c 1090  .d.<.|.d...}.|..
-00002eb0: 0173 d27c 0e64 1a3d 007c 1190 0173 ca7c  .s.|.d.=.|...s.|
-00002ec0: 0ea0 3964 1ba1 0164 0075 0090 0172 ca64  ..9d...d.u...r.d
-00002ed0: 1c7c 0e64 1b3c 0074 3374 347c 0a83 027c  .|.d.<.t3t4|...|
-00002ee0: 0e64 1d3c 006e 4c7c 096a 0974 3b75 0090  .d.<.nL|.j.t;u..
-00002ef0: 0172 fd74 157c 0188 0083 0290 0172 e774  .r.t.|.......r.t
-00002f00: 3374 347c 0a83 027c 016a 357c 096a 363c  3t4|...|.j5|.j6<
-00002f10: 0064 1e44 005d 097d 127c 0ea0 387c 1264  .d.D.].}.|..8|.d
-00002f20: 00a1 0201 0090 0171 e97c 0e64 1f19 0090  .......q.|.d....
-00002f30: 0173 fc74 3c7c 0e64 1f3c 006e 217c 096a  .s.t<|.d.<.n!|.j
-00002f40: 3d64 0e6b 0390 0272 0b74 3374 347c 0a83  =d.k...r.t3t4|..
-00002f50: 027c 0e64 1d3c 006e 137c 0a74 3e75 0090  .|.d.<.n.|.t>u..
-00002f60: 0272 1574 3f7c 0e64 1f3c 006e 097c 0a74  .r.t?|.d.<.n.|.t
-00002f70: 0b75 0090 0272 1e74 407c 0e64 1f3c 007c  .u...r.t@|.d.<.|
-00002f80: 086a 1e74 1f75 0190 0273 327c 086a 2074  .j.t.u...s2|.j t
-00002f90: 1f75 0190 0273 327c 0ea0 3964 20a1 0164  .u...s2|..9d ..d
-00002fa0: 0075 0190 0272 c97c 0ea0 3964 1fa1 0190  .u...r.|..9d....
-00002fb0: 0272 6574 247c 0e64 1f19 0074 416a 4274  .ret$|.d...tAjBt
-00002fc0: 3c66 0283 0290 0272 6574 0964 2164 2269  <f.....ret.d!d"i
-00002fd0: 0083 0383 007d 137c 0e64 1f19 007c 107c  .....}.|.d...|.|
-00002fe0: 0e64 1719 0064 238d 027c 017c 137c 0e64  .d...d#..|.|.|.d
-00002ff0: 2019 0064 248d 0301 0074 437c 137c 0e64   ..d$....tC|.|.d
-00003000: 1719 0083 027c 0e64 203c 006e 0f64 1d7c  .....|.d <.n.d.|
-00003010: 0e76 0090 0272 747c 0e64 1d19 007c 0e64  .v...rt|.d...|.d
-00003020: 2019 0083 017c 0e64 203c 007c 0ea0 3964   ....|.d <.|..9d
-00003030: 15a1 0190 0272 c97c 0e64 2019 007d 1474  .....r.|.d ..}.t
-00003040: 0a7c 1474 0b83 0290 0273 8c74 0a7c 1474  .|.t.....s.t.|.t
-00003050: 256a 266a 2a83 0290 0273 8f7c 1467 017d  %j&j*....s.|.g.}
-00003060: 147c 1444 005d 377d 0b7c 0b7c 0e64 1519  .|.D.]7}.|.|.d..
-00003070: 0076 0190 0272 c774 0a7c 0b74 3283 0290  .v...r.t.|.t2...
-00003080: 0272 a87c 0b6a 1c7c 0e64 1519 0076 0190  .r.|.j.|.d...v..
-00003090: 0272 c77c 0ea0 3964 1aa1 0190 0273 b37c  .r.|..9d.....s.|
-000030a0: 0b64 0075 0090 0273 c764 257c 0b9b 0064  .d.u...s.d%|...d
-000030b0: 267c 0e64 1719 009b 0064 277c 0e64 1519  &|.d.....d'|.d..
-000030c0: 009b 009d 067d 037c 01a0 047c 03a1 0101  .....}.|...|....
-000030d0: 0090 0271 9164 287c 0c9b 009d 0267 017d  ...q.d(|.....g.}
-000030e0: 157c 1190 0273 e674 157c 0ea0 3964 20a1  .|...s.t.|..9d .
-000030f0: 0174 0b83 0290 0272 e17c 15a0 4464 29a1  .t.....r.|..Dd).
-00003100: 0101 006e 057c 15a0 4464 2aa1 0101 007c  ...n.|..Dd*....|
-00003110: 0ea0 3864 2b64 0da1 0290 0272 f27c 15a0  ..8d+d.....r.|..
-00003120: 4464 2ca1 0101 007c 096a 4590 0272 ff7c  Dd,....|.jE..r.|
-00003130: 15a0 4464 2d7c 096a 459b 009d 02a1 0101  ..Dd-|.jE.......
-00003140: 0064 2e64 2fa0 467c 15a1 019b 009d 027d  .d.d/.F|.......}
-00003150: 167c 0ea0 3964 30a1 0190 0372 187c 0e64  .|..9d0....r.|.d
-00003160: 3005 0019 0064 317c 1617 0037 0003 003c  0....d1|...7...<
-00003170: 006e 047c 167c 0e64 303c 007c 0ea0 3864  .n.|.|.d0<.|..8d
-00003180: 3264 00a1 027d 177c 1790 0373 2c7c 1190  2d...}.|...s,|..
-00003190: 0372 2a64 336e 0164 347d 177c 04a0 397c  .r*d3n.d4}.|..9|
-000031a0: 1764 00a1 027d 187c 1890 0373 3e7c 01a0  .d...}.|...s>|..
-000031b0: 477c 17a1 017d 187c 187c 047c 173c 007c  G|...}.|.|.|.<.|
-000031c0: 096a 4890 0372 697c 1190 0372 5064 357c  .jH..ri|...rPd5|
-000031d0: 096a 369b 009d 027d 037c 01a0 047c 03a1  .j6....}.|...|..
-000031e0: 0101 007c 016a 497c 016a 4aa0 3988 006a  ...|.jI|.jJ.9..j
-000031f0: 4ba1 0119 007c 1719 00a0 447c 096a 367c  K....|....D|.j6|
-00003200: 1090 0372 657c 1064 0c19 006e 0164 0066  ...re|.d...n.d.f
-00003210: 02a1 0101 007c 186a 4c7c 1069 007c 0ea4  .....|.jL|.i.|..
-00003220: 018e 0101 007c 07a0 447c 09a1 0101 0071  .....|..D|.....q
-00003230: 3e7c 0753 0029 364e 7a3e 5468 6973 2070  >|.S.)6Nz>This p
-00003240: 6172 7365 7220 616c 7265 6164 7920 636f  arser already co
-00003250: 6e74 6169 6e73 2061 7267 756d 656e 7473  ntains arguments
-00003260: 2066 726f 6d20 616e 6f74 6865 7220 6461   from another da
-00003270: 7461 636c 6173 732e 6301 0000 0000 0000  taclass.c.......
-00003280: 0000 0000 0001 0000 0004 0000 0013 0000  ................
-00003290: 0073 1200 0000 8800 6a00 8801 7c00 6a01  .s......j...|.j.
-000032a0: 6401 8d02 0c00 5300 2902 4e72 a200 0000  d.....S.).Nr....
-000032b0: 2902 72a3 0000 0072 9000 0000 2901 da01  ).r....r....)...
-000032c0: 66a9 02da 0363 6c73 5a05 6d6f 6465 6c72  f....clsZ.modelr
-000032d0: 5300 0000 7257 0000 0072 5e00 0000 ae01  S...rW...r^.....
-000032e0: 0000 f302 0000 0012 007a 2f41 7267 756d  .........z/Argum
-000032f0: 656e 7450 6172 7365 722e 5f61 6464 5f61  entParser._add_a
-00003300: 7267 756d 656e 7473 2e3c 6c6f 6361 6c73  rguments.<locals
-00003310: 3e2e 3c6c 616d 6264 613e 6301 0000 0000  >.<lambda>c.....
-00003320: 0000 0000 0000 0002 0000 0007 0000 0053  ...............S
-00003330: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
-00003340: 7c01 7c01 6a00 a001 7402 7403 8300 a102  |.|.j...t.t.....
-00003350: 6602 9102 7102 5300 7253 0000 0029 04da  f...q.S.rS...)..
-00003360: 086d 6574 6164 6174 61da 0367 6574 7221  .metadata..getr!
-00003370: 0000 0072 2200 0000 7254 0000 0072 5300  ...r"...rT...rS.
-00003380: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
-00003390: 00b3 0100 0073 0800 0000 0600 0202 12ff  .....s..........
-000033a0: 06ff 7a31 4172 6775 6d65 6e74 5061 7273  ..z1ArgumentPars
-000033b0: 6572 2e5f 6164 645f 6172 6775 6d65 6e74  er._add_argument
-000033c0: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
-000033d0: 636f 6d70 3e72 3d00 0000 5429 01da 0d69  comp>r=...T)...i
-000033e0: 735f 756e 696f 6e5f 7479 7065 da01 2e72  s_union_type...r
-000033f0: 1700 0000 a901 da08 6d61 7873 706c 6974  ........maxsplit
-00003400: e9ff ffff ff46 7201 0000 0029 01da 1061  .....Fr....)...a
-00003410: 7373 6572 745f 7072 696d 6974 6976 6563  ssert_primitivec
-00003420: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00003430: 0300 0000 5300 0000 7312 0000 0067 007c  ....S...s....g.|
-00003440: 005d 057d 017c 016a 0091 0271 0253 0072  .].}.|.j...q.S.r
-00003450: 5300 0000 a901 7290 0000 0072 5400 0000  S.....r....rT...
-00003460: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-00003470: 5800 0000 0f02 0000 72a7 0000 00da 0370  X.......r......p
-00003480: 6f73 7267 0000 0063 0100 0000 0000 0000  osrg...c........
-00003490: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
-000034a0: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
-000034b0: 0064 00a1 0172 027c 0191 0271 0253 0029  .d...r.|...q.S.)
-000034c0: 0172 6500 0000 725f 0000 0072 5400 0000  .re...r_...rT...
-000034d0: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
-000034e0: 5800 0000 2902 0000 7302 0000 001a 00da  X...)...s.......
-000034f0: 076d 6574 6176 6172 7264 0000 00fa 013c  .metavarrd.....<
-00003500: da04 6465 7374 fa01 3e7a 073c 7661 6c75  ..dest..>z.<valu
-00003510: 653e da08 7265 7175 6972 6564 da05 6e61  e>..required..na
-00003520: 7267 73fa 013f da04 7479 7065 2905 72b9  rgs..?..type).r.
-00003530: 0000 0072 b700 0000 da05 636f 6e73 7472  ...r......constr
-00003540: 6400 0000 72b2 0000 0072 5900 0000 7263  d...r....rY...rc
-00003550: 0000 00da 0072 5300 0000 2902 7267 0000  .....rS...).rg..
-00003560: 0072 b400 0000 2903 7266 0000 00da 096e  .r....).rf.....n
-00003570: 616d 6573 7061 6365 da06 7661 6c75 6573  amespace..values
-00003580: 7a0f 496e 7661 6c69 6420 7661 6c75 6520  z.Invalid value 
-00003590: 277a 1027 2066 6f72 2061 7267 756d 656e  'z.' for argumen
-000035a0: 7420 277a 1327 3b20 6d75 7374 2062 6520  t 'z.'; must be 
-000035b0: 6f6e 6520 6f66 3a20 7a06 5479 7065 3a20  one of: z.Type: 
-000035c0: 7a16 4465 6661 756c 743a 2022 2528 6465  z.Default: "%(de
-000035d0: 6661 756c 7429 7322 7a14 4465 6661 756c  fault)s"z.Defaul
-000035e0: 743a 2025 2864 6566 6175 6c74 2973 da09  t: %(default)s..
-000035f0: 6578 636c 7573 6976 657a 044d 2e58 2e7a  exclusivez.M.X.z
-00003600: 0545 6e76 3a20 7a02 3e20 fa02 2c20 725a  .Env: z.> .., rZ
-00003610: 0000 0072 7b00 0000 da05 6772 6f75 707a  ...r{.....groupz
-00003620: 1372 6571 7569 7265 6420 7061 7261 6d65  .required parame
-00003630: 7465 7273 7a13 6f70 7469 6f6e 616c 2070  tersz.optional p
-00003640: 6172 616d 6574 6572 737a 3341 206d 7574  arametersz3A mut
-00003650: 7561 6c6c 792d 6578 636c 7573 6976 6520  ually-exclusive 
-00003660: 7061 7261 6d65 7465 7220 6361 6e6e 6f74  parameter cannot
-00003670: 2062 6520 7265 7175 6972 6564 3a20 294d   be required: )M
-00003680: 7234 0000 0072 2500 0000 da0b 6765 745f  r4...r%.....get_
-00003690: 6465 6661 756c 7472 4600 0000 7280 0000  defaultrF...r...
-000036a0: 0072 9c00 0000 725d 0000 00da 0666 696c  .r....r].....fil
-000036b0: 7465 7272 0600 0000 72b9 0000 0072 3800  terr....r....r8.
-000036c0: 0000 726d 0000 0072 2300 0000 727d 0000  ..rm...r#...r}..
-000036d0: 00da 0c76 6572 7369 6f6e 5f69 6e66 6f72  ...version_infor
-000036e0: 3f00 0000 da10 5f67 6574 5f74 7970 655f  ?....._get_type_
-000036f0: 6f72 6967 696e 7215 0000 00da 1c5f 6578  originr......_ex
-00003700: 7472 6163 745f 7479 7065 5f66 726f 6d5f  tract_type_from_
-00003710: 636f 6e74 6169 6e65 7272 3c00 0000 da12  containerr<.....
-00003720: 5f67 6574 5f74 7970 655f 6d65 7461 6461  _get_type_metada
-00003730: 7461 726c 0000 0072 0500 0000 7221 0000  tarl...r....r!..
-00003740: 0072 a800 0000 7294 0000 00da 0672 7370  .r....r......rsp
-00003750: 6c69 74da 0873 6574 5f64 6573 7472 9000  lit..set_destr..
-00003760: 0000 72b6 0000 0072 6300 0000 7204 0000  ..r....rc...r...
-00003770: 00da 0f64 6566 6175 6c74 5f66 6163 746f  ...default_facto
-00003780: 7279 722a 0000 00da 0e5f 6765 745f 7479  ryr*....._get_ty
-00003790: 7065 5f61 7267 7372 6400 0000 7239 0000  pe_argsrd...r9..
-000037a0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
-000037b0: 6162 63da 074d 6170 7069 6e67 7259 0000  abc..MappingrY..
-000037c0: 0072 1d00 0000 da08 4974 6572 6162 6c65  .r......Iterable
-000037d0: da03 7365 7472 1f00 0000 da05 7475 706c  ..setr......tupl
-000037e0: 6572 2000 0000 721e 0000 0072 3500 0000  er ...r....r5...
-000037f0: 7227 0000 0072 0700 0000 7208 0000 0072  r'...r....r....r
-00003800: 3100 0000 7271 0000 0072 b400 0000 da06  1...rq...r......
-00003810: 6173 6469 6374 7296 0000 0072 a900 0000  asdictr....r....
-00003820: da05 7570 7065 72da 0462 6f6f 6c72 1800  ..upper..boolr..
-00003830: 0000 72b7 0000 00da 0369 6e74 7219 0000  ..r......intr...
-00003840: 0072 1a00 0000 7273 0000 00da 0641 6374  .r....rs.....Act
-00003850: 696f 6eda 0767 6574 6174 7472 da06 6170  ion..getattr..ap
-00003860: 7065 6e64 da08 5f65 6e76 5f76 6172 da04  pend.._env_var..
-00003870: 6a6f 696e da12 6164 645f 6172 6775 6d65  join..add_argume
-00003880: 6e74 5f67 726f 7570 72be 0000 0072 7000  nt_groupr....rp.
-00003890: 0000 da09 5f64 6566 6175 6c74 7372 4500  ...._defaultsrE.
-000038a0: 0000 726e 0000 0029 1972 a600 0000 7266  ..rn...).r....rf
-000038b0: 0000 0072 8d00 0000 da03 6572 725a 1170  ...r......errZ.p
-000038c0: 6172 7365 725f 6172 675f 6772 6f75 7073  arser_arg_groups
-000038d0: 5a0c 6e6f 7665 6c5f 6669 656c 6473 5a10  Z.novel_fieldsZ.
-000038e0: 6e6f 7665 6c5f 6669 656c 645f 6172 6773  novel_field_args
-000038f0: 5a0a 6164 6465 645f 6172 6773 5a03 666c  Z.added_argsZ.fl
-00003900: 645a 1161 7267 7061 7273 655f 6172 6775  dZ.argparse_argu
-00003910: 6d65 6e74 da08 666c 645f 7479 7065 7256  ment..fld_typerV
-00003920: 0000 005a 0968 656c 705f 7479 7065 5a0f  ...Z.help_typeZ.
-00003930: 666c 645f 7479 7065 5f6f 7269 6769 6e72  fld_type_originr
-00003940: 5100 0000 7267 0000 0072 5000 0000 72b6  Q...rg...rP...r.
-00003950: 0000 00da 016b 5a0f 6475 6d6d 795f 6e61  .....kZ.dummy_na
-00003960: 6d65 7370 6163 65da 0164 5a0e 6865 6c70  mespace..dZ.help
-00003970: 5f6d 7367 5f70 6172 7473 5a08 6865 6c70  _msg_partsZ.help
-00003980: 5f6d 7367 72c0 0000 005a 0961 7267 5f67  _msgr....Z.arg_g
-00003990: 726f 7570 7253 0000 0072 a500 0000 7257  rouprS...r....rW
-000039a0: 0000 0072 8e00 0000 9501 0000 739c 0100  ...r........s...
-000039b0: 0008 0a06 0108 020c 0204 010a 0116 0204  ................
-000039c0: 0202 0202 010c 0106 0102 fe04 ff06 0702  ................
-000039d0: 0206 fe04 050e 0206 010a 0408 010e 0114  ................
-000039e0: 030e 0104 0102 0102 0106 fe0a 050e 0114  ................
-000039f0: 010a 0104 0102 800a 0214 030e 0104 0102  ................
-00003a00: 0102 0106 fe08 0708 ff14 0202 fd0c 0606  ................
-00003a10: 020a 0108 0108 010a 010a 0106 010a 0206  ................
-00003a20: 0110 0110 0108 010e 0102 8010 0304 0102  ................
-00003a30: 0102 0106 fe08 0406 0102 800c 0304 ff0a  ................
-00003a40: 0204 0202 0102 0106 fe08 040a 0108 010a  ................
-00003a50: 0108 0106 0202 8006 0208 010c 0210 010c  ................
-00003a60: 0202 0302 0102 010c fe06 070c 020a 0106  ................
-00003a70: 0208 0206 010a 0202 0308 ff0c 0202 fd16  ................
-00003a80: 061c 0206 ff08 0406 0206 0216 0108 0110  ................
-00003a90: 010c 010c 0102 0302 0102 010c fe08 0510  ................
-00003aa0: 010a 0108 0102 800c 0210 010a 010a 020a  ................
-00003ab0: 0108 020c 040c 0110 010e 0206 0108 0106  ................
-00003ac0: fe0e 0512 0102 0102 0106 0106 fd14 050a  ................
-00003ad0: 0114 010c 0308 010e 0102 0106 0106 fe06  ................
-00003ae0: 0408 020e 0208 0204 fe10 0308 0304 fd0a  ................
-00003af0: 0312 0306 0104 ff02 ff0a 0404 800c 0206  ................
-00003b00: 0312 010c 010a 020e 020a 0108 0212 0110  ................
-00003b10: 020c 0216 0108 020c 0206 020e 010c 0206  ................
-00003b20: 020a 0108 0108 0206 0102 0204 0104 ff02  ................
-00003b30: ff0a 0404 020c 0102 ff02 0202 fe02 0204  ................
-00003b40: 0210 0102 fe04 ff10 070c 0204 027a 1d41  .............z.A
-00003b50: 7267 756d 656e 7450 6172 7365 722e 5f61  rgumentParser._a
-00003b60: 6464 5f61 7267 756d 656e 7473 da01 7463  dd_arguments..tc
-00003b70: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-00003b80: 0400 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
-00003b90: 0064 0164 0083 0353 0029 024e da0a 5f5f  .d.d...S.).N..__
-00003ba0: 6f72 6967 696e 5f5f a901 72d6 0000 00a9  origin__..r.....
-00003bb0: 0172 e000 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-00003bc0: 7257 0000 0072 c400 0000 b602 0000 f302  rW...r..........
-00003bd0: 0000 000c 027a 1f41 7267 756d 656e 7450  .....z.ArgumentP
-00003be0: 6172 7365 722e 5f67 6574 5f74 7970 655f  arser._get_type_
-00003bf0: 6f72 6967 696e 6301 0000 0000 0000 0000  originc.........
-00003c00: 0000 0001 0000 0004 0000 0043 0000 00f3  ...........C....
-00003c10: 0c00 0000 7400 7c00 6401 6402 8303 5300  ....t.|.d.d...S.
-00003c20: 2903 4eda 085f 5f61 7267 735f 5f72 5300  ).N..__args__rS.
-00003c30: 0000 72e2 0000 0072 e300 0000 7253 0000  ..r....r....rS..
-00003c40: 0072 5300 0000 7257 0000 0072 ca00 0000  .rS...rW...r....
-00003c50: ba02 0000 72e4 0000 007a 1d41 7267 756d  ....r....z.Argum
-00003c60: 656e 7450 6172 7365 722e 5f67 6574 5f74  entParser._get_t
-00003c70: 7970 655f 6172 6773 6301 0000 0000 0000  ype_argsc.......
-00003c80: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00003c90: 0072 e500 0000 2903 4eda 0c5f 5f6d 6574  .r....).N..__met
-00003ca0: 6164 6174 615f 5f72 5300 0000 72e2 0000  adata__rS...r...
-00003cb0: 0072 e300 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-00003cc0: 7257 0000 0072 c600 0000 be02 0000 72e4  rW...r........r.
-00003cd0: 0000 007a 2141 7267 756d 656e 7450 6172  ...z!ArgumentPar
-00003ce0: 7365 722e 5f67 6574 5f74 7970 655f 6d65  ser._get_type_me
-00003cf0: 7461 6461 7461 da0e 7479 7065 5f63 6f6e  tadata..type_con
-00003d00: 7461 696e 6572 72af 0000 0072 aa00 0000  tainerr....r....
-00003d10: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
-00003d20: 0003 0000 0043 0000 0073 1801 0000 7c03  .....C...s....|.
-00003d30: 7204 7400 6e04 7c00 a001 7c01 a101 7d04  r.t.n.|...|...}.
-00003d40: 7c04 6400 7500 7215 7402 6401 7c01 6a03  |.d.u.r.t.d.|.j.
-00003d50: 9b00 9d02 8301 8201 7c00 a004 7c01 a101  ........|...|...
-00003d60: 7d05 6402 6403 8400 7c05 4400 8301 7d06  }.d.d...|.D...}.
-00003d70: 7c04 7400 7500 7330 7405 7c04 7406 6a07  |.t.u.s0t.|.t.j.
-00003d80: 6a08 8302 7330 7c04 7409 7500 7240 740a  j...s0|.t.u.r@t.
-00003d90: 7c06 8301 6404 6b03 723b 7c06 a00b a100  |...d.k.r;|.....
-00003da0: 0100 6e2c 7c06 6405 1900 7d07 6e27 7405  ..n,|.d...}.n't.
-00003db0: 7c04 7406 6a07 6a0c 8302 7261 740a 7c06  |.t.j.j...rat.|.
-00003dc0: 8301 6406 6b03 7252 7c06 a00b a100 0100  ..d.k.rR|.......
-00003dd0: 6e15 7c06 5c02 7d08 7d09 7c08 740d 7501  n.|.\.}.}.|.t.u.
-00003de0: 725e 7402 6407 8301 8201 7c09 7d07 6e06  r^t.d.....|.}.n.
-00003df0: 740e 7367 740f 7c01 8301 0100 7c06 736d  t.sgt.|.....|.sm
-00003e00: 7402 6408 8301 8201 7c00 a001 7c07 a101  t.d.....|...|...
-00003e10: 7d0a 7c0a 7400 7500 7280 7c00 a010 7c07  }.|.t.u.r.|...|.
-00003e20: a101 7d07 7c00 a001 7c07 a101 7d0a 7c02  ..}.|...|...}.|.
-00003e30: 728a 7c0a 728a 740e 738a 740f 7c0a 8301  r.|.r.t.s.t.|...
-00003e40: 0100 7c07 5300 2909 4e7a 1f47 6976 656e  ..|.S.).Nz.Given
-00003e50: 2074 7970 6520 6973 206e 6f74 2061 2063   type is not a c
-00003e60: 6f6e 7461 696e 6572 3a20 6301 0000 0000  ontainer: c.....
-00003e70: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
-00003e80: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
-00003e90: 7c01 6400 7501 7202 7c01 7400 7501 7202  |.d.u.r.|.t.u.r.
-00003ea0: 7c01 9102 7102 5300 2901 2e29 0172 2b00  |...q.S.)..).r+.
-00003eb0: 0000 2902 7255 0000 00da 0161 7253 0000  ..).rU.....arS..
-00003ec0: 0072 5300 0000 7257 0000 0072 5800 0000  .rS...rW...rX...
-00003ed0: d402 0000 7304 0000 0006 001a 017a 3f41  ....s........z?A
-00003ee0: 7267 756d 656e 7450 6172 7365 722e 5f65  rgumentParser._e
-00003ef0: 7874 7261 6374 5f74 7970 655f 6672 6f6d  xtract_type_from
-00003f00: 5f63 6f6e 7461 696e 6572 2e3c 6c6f 6361  _container.<loca
-00003f10: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7217  ls>.<listcomp>r.
-00003f20: 0000 0072 0100 0000 727a 0000 007a 2244  ...r....rz...z"D
-00003f30: 6963 7469 6f6e 6172 7920 6b65 7973 206d  ictionary keys m
-00003f40: 7573 7420 6265 2074 7970 6520 6073 7472  ust be type `str
-00003f50: 607a 1b54 6f6f 206d 616e 7920 7479 7065  `z.Too many type
-00003f60: 7320 696e 2063 6f6e 7461 696e 6572 2911  s in container).
-00003f70: 7215 0000 0072 c400 0000 da09 5479 7065  r....r......Type
-00003f80: 4572 726f 7272 9400 0000 72ca 0000 0072  Errorr....r....r
-00003f90: 3900 0000 72cb 0000 0072 cc00 0000 7211  9...r....r....r.
-00003fa0: 0000 0072 cf00 0000 7275 0000 00da 0563  ...r....ru.....c
-00003fb0: 6c65 6172 72cd 0000 0072 6d00 0000 7235  learr....rm...r5
-00003fc0: 0000 0072 2700 0000 72c5 0000 0029 0b72  ...r'...r....).r
-00003fd0: a600 0000 72e8 0000 0072 af00 0000 72aa  ....r....r....r.
-00003fe0: 0000 005a 1574 7970 655f 636f 6e74 6169  ...Z.type_contai
-00003ff0: 6e65 725f 6f72 6967 696e 5a13 7479 7065  ner_originZ.type
-00004000: 5f63 6f6e 7461 696e 6572 5f61 7267 73da  _container_args.
-00004010: 0772 6573 756c 7473 5a16 7479 7065 5f63  .resultsZ.type_c
-00004020: 6f6e 7461 696e 6572 5f73 7562 7479 7065  ontainer_subtype
-00004030: 5a08 6b65 795f 7479 7065 5a0a 7661 6c75  Z.key_typeZ.valu
-00004040: 655f 7479 7065 5a1d 7479 7065 5f63 6f6e  e_typeZ.type_con
-00004050: 7461 696e 6572 5f73 7562 7479 7065 5f6f  tainer_subtype_o
-00004060: 7269 6769 6e72 5300 0000 7253 0000 0072  riginrS...rS...r
-00004070: 5700 0000 72c5 0000 00c2 0200 0073 5400  W...r........sT.
-00004080: 0000 1008 02ff 0804 0201 0a01 04ff 0a04  ................
-00004090: 0602 0201 06ff 0807 0c01 02ff 0802 0c02  ................
-000040a0: 0a01 0a02 0e01 0c01 0a01 0802 0801 0801  ................
-000040b0: 0601 0401 0801 0402 0801 0a02 0802 0401  ................
-000040c0: 0201 04ff 0a03 0203 02ff 0202 02fe 0203  ................
-000040d0: 02fd 0805 0402 7a2b 4172 6775 6d65 6e74  ......z+Argument
-000040e0: 5061 7273 6572 2e5f 6578 7472 6163 745f  Parser._extract_
-000040f0: 7479 7065 5f66 726f 6d5f 636f 6e74 6169  type_from_contai
-00004100: 6e65 7263 0100 0000 0000 0000 0000 0000  nerc............
-00004110: 0200 0000 0400 0000 4300 0000 7324 0000  ........C...s$..
-00004120: 007c 006a 0044 005d 0c7d 0174 017c 0174  .|.j.D.].}.t.|.t
-00004130: 026a 0383 0272 0f7c 0102 0001 0053 0071  .j...r.|.....S.q
-00004140: 0364 0053 0072 5c00 0000 2904 da08 5f61  .d.S.r\...)..._a
-00004150: 6374 696f 6e73 726c 0000 0072 7300 0000  ctionsrl...rs...
-00004160: 7295 0000 0029 0272 7600 0000 72e9 0000  r....).rv...r...
-00004170: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
-00004180: 7289 0000 0002 0300 0073 1000 0000 0a01  r........s......
-00004190: 0201 0201 0401 04fe 0804 02fc 0405 7a1e  ..............z.
-000041a0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-000041b0: 6765 745f 7375 6270 6172 7365 7273 6301  get_subparsersc.
-000041c0: 0000 0000 0000 0000 0000 0002 0000 0007  ................
-000041d0: 0000 0003 0000 0073 2c00 0000 8800 a000  .......s,.......
-000041e0: a100 7d01 7c01 7314 8800 6a01 6401 6402  ..}.|.s...j.d.d.
-000041f0: 8800 6a02 8700 6601 6403 6404 8408 6405  ..j...f.d.d...d.
-00004200: 8d04 7d01 7c01 5300 2906 4e5a 0863 6f6d  ..}.|.S.).NZ.com
-00004210: 6d61 6e64 737a 093c 434f 4d4d 414e 443e  mandsz.<COMMAND>
-00004220: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
-00004230: 0006 0000 001b 0000 0073 1e00 0000 7400  .........s....t.
-00004240: 8800 8301 6403 6900 7c00 a401 6401 8800  ....d.i.|...d...
-00004250: 6a01 6402 9c02 a401 8e01 5300 2904 4e54  j.d.......S.).NT
-00004260: 2902 724f 0000 0072 4e00 0000 7253 0000  ).rO...rN...rS..
-00004270: 0029 0272 b900 0000 724e 0000 0029 0172  .).r....rN...).r
-00004280: de00 0000 a901 7276 0000 0072 5300 0000  ......rv...rS...
-00004290: 7257 0000 0072 5e00 0000 1303 0000 730c  rW...r^.......s.
-000042a0: 0000 000a 0002 0102 ff02 0204 010a fd7a  ...............z
-000042b0: 3741 7267 756d 656e 7450 6172 7365 722e  7ArgumentParser.
-000042c0: 5f67 6574 5f6f 725f 6164 645f 7375 6270  _get_or_add_subp
-000042d0: 6172 7365 7273 2e3c 6c6f 6361 6c73 3e2e  arsers.<locals>.
-000042e0: 3c6c 616d 6264 613e 2904 726b 0000 0072  <lambda>).rk...r
-000042f0: b200 0000 72b4 0000 00da 0c70 6172 7365  ....r......parse
-00004300: 725f 636c 6173 7329 0372 8900 0000 da0e  r_class).r......
-00004310: 6164 645f 7375 6270 6172 7365 7273 7244  add_subparsersrD
-00004320: 0000 0029 0272 7600 0000 728c 0000 0072  ...).rv...r....r
-00004330: 5300 0000 72ee 0000 0072 5700 0000 7293  S...r....rW...r.
-00004340: 0000 000b 0300 0073 1200 0000 0801 0402  .......s........
-00004350: 0401 0201 0201 0401 0a01 06fc 040b 7a25  ..............z%
-00004360: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00004370: 6765 745f 6f72 5f61 6464 5f73 7562 7061  get_or_add_subpa
-00004380: 7273 6572 7372 bc00 0000 6302 0000 0000  rsersr....c.....
-00004390: 0000 0000 0000 0006 0000 0006 0000 0003  ................
-000043a0: 0000 0073 6e00 0000 7c00 6a00 a001 7402  ...sn...|.j...t.
-000043b0: 8800 7c00 6a03 6400 8303 6900 a102 7d02  ..|.j.d...i...}.
-000043c0: 7c02 a004 a100 4400 5d1d 7d03 8700 6601  |.....D.].}...f.
-000043d0: 6401 6402 8408 7c03 4400 8301 7d04 7405  d.d...|.D...}.t.
-000043e0: 7c04 8301 6403 6b04 722d 6404 6405 a006  |...d.k.r-d.d...
-000043f0: 7c04 a101 1700 7d05 7c00 a007 7c05 a101  |.....}.|...|...
-00004400: 0100 7110 7408 6406 6900 7409 8800 8301  ..q.t.d.i.t.....
-00004410: a401 8e01 5300 2907 4e63 0100 0000 0000  ....S.).Nc......
-00004420: 0000 0000 0000 0400 0000 0500 0000 1300  ................
-00004430: 0000 736c 0000 0067 007c 005d 325c 027d  ..sl...g.|.]2\.}
-00004440: 017d 0274 0088 007c 0183 0272 3474 0188  .}.t...|...r4t..
-00004450: 007c 0183 027d 0374 027c 0374 0383 0273  .|...}.t.|.t...s
-00004460: 1c74 027c 0374 046a 056a 0683 0273 207c  .t.|.t.j.j...s |
-00004470: 0364 0075 0173 2e74 027c 0374 0383 0273  .d.u.s.t.|.t...s
-00004480: 0274 027c 0374 046a 056a 0683 0272 027c  .t.|.t.j.j...r.|
-00004490: 0372 027c 0272 327c 026e 017c 0191 0271  .r.|.r2|.n.|...q
-000044a0: 0253 0072 5c00 0000 2907 da07 6861 7361  .S.r\...)...hasa
-000044b0: 7474 7272 d600 0000 7238 0000 0072 6d00  ttrr....r8...rm.
-000044c0: 0000 72cb 0000 0072 cc00 0000 72ce 0000  ..r....r....r...
-000044d0: 0029 0472 5500 0000 72b4 0000 00da 0466  .).rU...r......f
-000044e0: 6c61 675a 0a61 7474 725f 7661 6c75 65a9  lagZ.attr_value.
-000044f0: 0172 bc00 0000 7253 0000 0072 5700 0000  .r....rS...rW...
-00004500: 7258 0000 002b 0300 0073 3000 0000 0600  rX...+...s0.....
-00004510: 0602 0801 02fd 0a04 0803 02f9 0208 0201  ................
-00004520: 0601 02fe 02f8 080d 0803 02fd 0204 0201  ................
-00004530: 0601 02fe 02fc 0208 02f8 0af4 060c 7a33  ..............z3
-00004540: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
-00004550: 706f 7374 5f70 6172 7365 5f61 7267 732e  post_parse_args.
-00004560: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
-00004570: 6d70 3e72 1700 0000 7a28 5468 6573 6520  mp>r....z(These 
-00004580: 6172 6775 6d65 6e74 7320 6172 6520 6d75  arguments are mu
-00004590: 7475 616c 6c79 2065 7863 6c75 7369 7665  tually exclusive
-000045a0: 3a20 72bf 0000 0072 5300 0000 290a 7270  : r....rS...).rp
-000045b0: 0000 0072 a900 0000 72d6 0000 0072 4500  ...r....r....rE.
-000045c0: 0000 72bd 0000 0072 7500 0000 72d9 0000  ..r....ru...r...
-000045d0: 0072 8000 0000 7228 0000 00da 0476 6172  .r....r(.....var
-000045e0: 7329 0672 7600 0000 72bc 0000 005a 1266  s).rv...r....Z.f
-000045f0: 756e 635f 6d78 5f61 7267 5f67 726f 7570  unc_mx_arg_group
-00004600: 735a 0667 5f61 7267 735a 0e6d 785f 666c  sZ.g_argsZ.mx_fl
-00004610: 6167 735f 666f 756e 6472 dc00 0000 7253  ags_foundr....rS
-00004620: 0000 0072 f300 0000 7257 0000 00da 105f  ...r....rW....._
-00004630: 706f 7374 5f70 6172 7365 5f61 7267 731c  post_parse_args.
-00004640: 0300 0073 2000 0000 0607 0c01 0201 02fe  ...s ...........
-00004650: 02fd 0c07 0a04 0202 06fe 0c19 0601 0201  ................
-00004660: 06ff 0a03 0280 1202 7a1f 4172 6775 6d65  ........z.Argume
-00004670: 6e74 5061 7273 6572 2e5f 706f 7374 5f70  ntParser._post_p
-00004680: 6172 7365 5f61 7267 7363 0300 0000 0000  arse_argsc......
-00004690: 0000 0000 0000 0500 0000 0a00 0000 0300  ................
-000046a0: 0000 7352 0000 007a 0e74 0083 006a 017c  ..sR...z.t...j.|
-000046b0: 017c 0264 018d 027d 037c 00a0 027c 03a1  .|.d...}.|...|..
-000046c0: 0157 0053 0004 0074 0379 2801 007d 0401  .W.S...t.y(..}..
-000046d0: 007a 0e7c 00a0 0474 057c 0483 01a1 0101  .z.|...t.|......
-000046e0: 0057 0059 0064 007d 047e 0464 0053 0064  .W.Y.d.}.~.d.S.d
-000046f0: 007d 047e 0477 0177 00a9 024e 2902 7250  .}.~.w.w...N).rP
-00004700: 0000 0072 bc00 0000 2906 7268 0000 00da  ...r....).rh....
-00004710: 0a70 6172 7365 5f61 7267 7372 f500 0000  .parse_argsr....
-00004720: da0a 5661 6c75 6545 7272 6f72 7280 0000  ..ValueErrorr...
-00004730: 0072 6d00 0000 2905 7276 0000 0072 5000  .rm...).rv...rP.
-00004740: 0000 72bc 0000 00da 0670 6172 7365 64da  ..r......parsed.
-00004750: 0165 7277 0000 0072 5300 0000 7257 0000  .erw...rS...rW..
-00004760: 0072 f700 0000 4c03 0000 7314 0000 0002  .r....L...s.....
-00004770: 0506 0102 0102 0106 fe0c 040e 011c 0108  ................
-00004780: 8002 ff7a 1941 7267 756d 656e 7450 6172  ...z.ArgumentPar
-00004790: 7365 722e 7061 7273 655f 6172 6773 6303  ser.parse_argsc.
-000047a0: 0000 0000 0000 0000 0000 0006 0000 000a  ................
-000047b0: 0000 0003 0000 0073 5a00 0000 7a12 7400  .......sZ...z.t.
-000047c0: 8300 6a01 7c01 7c02 6401 8d02 5c02 7d03  ..j.|.|.d...\.}.
-000047d0: 7d04 7c00 a002 7c03 a101 7c04 6602 5700  }.|...|...|.f.W.
-000047e0: 5300 0400 7403 792c 0100 7d05 0100 7a0e  S...t.y,..}...z.
-000047f0: 7c00 a004 7405 7c05 8301 a101 0100 5700  |...t.|.......W.
-00004800: 5900 6400 7d05 7e05 6400 5300 6400 7d05  Y.d.}.~.d.S.d.}.
-00004810: 7e05 7701 7700 72f6 0000 0029 0672 6800  ~.w.w.r....).rh.
-00004820: 0000 da10 7061 7273 655f 6b6e 6f77 6e5f  ....parse_known_
-00004830: 6172 6773 72f5 0000 0072 f800 0000 7280  argsr....r....r.
-00004840: 0000 0072 6d00 0000 2906 7276 0000 0072  ...rm...).rv...r
-00004850: 5000 0000 72bc 0000 0072 f900 0000 da07  P...r....r......
-00004860: 756e 6b6e 6f77 6e72 fa00 0000 7277 0000  unknownr....rw..
-00004870: 0072 5300 0000 7257 0000 0072 fb00 0000  .rS...rW...r....
-00004880: 5a03 0000 730e 0000 0002 0714 0110 010e  Z...s...........
-00004890: 011c 0108 8002 ff7a 1f41 7267 756d 656e  .......z.Argumen
-000048a0: 7450 6172 7365 722e 7061 7273 655f 6b6e  tParser.parse_kn
-000048b0: 6f77 6e5f 6172 6773 da18 736b 6970 5f70  own_args..skip_p
-000048c0: 7964 616e 7469 635f 7661 6c69 6461 7469  ydantic_validati
-000048d0: 6f6e 6304 0000 0000 0000 0000 0000 0006  onc.............
-000048e0: 0000 0005 0000 0043 0000 0073 2200 0000  .......C...s"...
-000048f0: 7c00 a000 7c01 a101 5c02 7d04 7d05 7c00  |...|...\.}.}.|.
-00004900: 6a01 7c04 7c02 7c03 6401 8d03 7c05 6602  j.|.|.|.d...|.f.
-00004910: 5300 2902 61c9 0200 0055 7365 2070 6172  S.).a....Use par
-00004920: 7365 6420 6172 6773 2074 6f20 696e 7374  sed args to inst
-00004930: 616e 7469 6174 6520 7468 6520 6769 7665  antiate the give
-00004940: 6e20 6461 7461 206d 6f64 656c 2e0a 0a20  n data model... 
-00004950: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00004960: 2020 2020 2020 2020 2061 7267 733a 0a20           args:. 
-00004970: 2020 2020 2020 2020 2020 2061 7267 735f             args_
-00004980: 6d6f 6465 6c3a 0a20 2020 2020 2020 2020  model:.         
-00004990: 2020 2073 6b69 705f 7079 6461 6e74 6963     skip_pydantic
-000049a0: 5f76 616c 6964 6174 696f 6e3a 0a0a 2020  _validation:..  
-000049b0: 2020 2020 2020 4578 616d 706c 6573 3a0a        Examples:.
-000049c0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-000049d0: 696d 706f 7274 2079 6170 780a 2020 2020  import yapx.    
-000049e0: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
-000049f0: 2064 6174 6163 6c61 7373 6573 2069 6d70   dataclasses imp
-00004a00: 6f72 7420 6461 7461 636c 6173 730a 2020  ort dataclass.  
-00004a10: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00004a20: 2020 2020 2020 2020 2020 3e3e 3e20 4064            >>> @d
-00004a30: 6174 6163 6c61 7373 0a20 2020 2020 2020  ataclass.       
-00004a40: 2020 2020 202e 2e2e 2063 6c61 7373 2041       ... class A
-00004a50: 6464 4e75 6d73 3a0a 2020 2020 2020 2020  ddNums:.        
-00004a60: 2020 2020 2e2e 2e20 2020 2020 783a 2069      ...     x: i
-00004a70: 6e74 0a20 2020 2020 2020 2020 2020 202e  nt.            .
-00004a80: 2e2e 2020 2020 2079 3a20 696e 740a 2020  ..     y: int.  
-00004a90: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00004aa0: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
-00004ab0: 7273 6572 203d 2079 6170 782e 4172 6775  rser = yapx.Argu
-00004ac0: 6d65 6e74 5061 7273 6572 2829 0a20 2020  mentParser().   
-00004ad0: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
-00004ae0: 7365 722e 6164 645f 6172 6775 6d65 6e74  ser.add_argument
-00004af0: 7328 4164 644e 756d 7329 0a20 2020 2020  s(AddNums).     
-00004b00: 2020 2020 2020 203e 3e3e 2070 6172 7365         >>> parse
-00004b10: 642c 2075 6e6b 6e6f 776e 203d 2070 6172  d, unknown = par
-00004b20: 7365 722e 7061 7273 655f 6b6e 6f77 6e5f  ser.parse_known_
-00004b30: 6172 6773 5f74 6f5f 6d6f 6465 6c28 5b27  args_to_model(['
-00004b40: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
-00004b50: 2732 272c 2027 2d7a 272c 2027 3327 5d29  '2', '-z', '3'])
-00004b60: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00004b70: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00004b80: 2028 7061 7273 6564 2e78 2c20 7061 7273   (parsed.x, pars
-00004b90: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
-00004ba0: 2020 2831 2c20 3229 0a20 2020 2020 2020    (1, 2).       
-00004bb0: 2020 2020 203e 3e3e 2075 6e6b 6e6f 776e       >>> unknown
-00004bc0: 0a20 2020 2020 2020 2020 2020 205b 272d  .            ['-
-00004bd0: 7a27 2c20 2733 275d 0a0a 2020 2020 2020  z', '3']..      
-00004be0: 2020 a903 7250 0000 0072 8d00 0000 72fd    ..rP...r....r.
-00004bf0: 0000 0029 0272 fb00 0000 da14 5f70 6172  ...).r......_par
-00004c00: 7365 5f61 7267 735f 746f 5f6d 6f64 656c  se_args_to_model
-00004c10: 2906 7276 0000 0072 5000 0000 728d 0000  ).rv...rP...r...
-00004c20: 0072 fd00 0000 da0b 7061 7273 6564 5f61  .r......parsed_a
-00004c30: 7267 73da 0c75 6e6b 6e6f 776e 5f61 7267  rgs..unknown_arg
-00004c40: 7372 5300 0000 7253 0000 0072 5700 0000  srS...rS...rW...
-00004c50: da19 7061 7273 655f 6b6e 6f77 6e5f 6172  ..parse_known_ar
-00004c60: 6773 5f74 6f5f 6d6f 6465 6c67 0300 0073  gs_to_modelg...s
-00004c70: 1000 0000 0e23 0403 0201 0201 0201 04fd  .....#..........
-00004c80: 0205 04fa 7a28 4172 6775 6d65 6e74 5061  ....z(ArgumentPa
-00004c90: 7273 6572 2e70 6172 7365 5f6b 6e6f 776e  rser.parse_known
-00004ca0: 5f61 7267 735f 746f 5f6d 6f64 656c 6304  _args_to_modelc.
-00004cb0: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00004cc0: 0000 0043 0000 0073 1a00 0000 7c00 a000  ...C...s....|...
-00004cd0: 7c01 a101 7d04 7c00 6a01 7c04 7c02 7c03  |...}.|.j.|.|.|.
-00004ce0: 6401 8d03 5300 2902 617f 0200 0055 7365  d...S.).a....Use
-00004cf0: 2070 6172 7365 6420 6172 6773 2074 6f20   parsed args to 
-00004d00: 696e 7374 616e 7469 6174 6520 7468 6520  instantiate the 
-00004d10: 6769 7665 6e20 6461 7461 206d 6f64 656c  given data model
-00004d20: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00004d30: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-00004d40: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00004d50: 7267 735f 6d6f 6465 6c3a 0a20 2020 2020  rgs_model:.     
-00004d60: 2020 2020 2020 2073 6b69 705f 7079 6461         skip_pyda
-00004d70: 6e74 6963 5f76 616c 6964 6174 696f 6e3a  ntic_validation:
-00004d80: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00004d90: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00004da0: 3e3e 3e20 696d 706f 7274 2079 6170 780a  >>> import yapx.
-00004db0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00004dc0: 6672 6f6d 2064 6174 6163 6c61 7373 6573  from dataclasses
-00004dd0: 2069 6d70 6f72 7420 6461 7461 636c 6173   import dataclas
-00004de0: 730a 2020 2020 2020 2020 2020 2020 2e2e  s.            ..
-00004df0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00004e00: 3e20 4064 6174 6163 6c61 7373 0a20 2020  > @dataclass.   
-00004e10: 2020 2020 2020 2020 202e 2e2e 2063 6c61           ... cla
-00004e20: 7373 2041 6464 4e75 6d73 3a0a 2020 2020  ss AddNums:.    
-00004e30: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00004e40: 783a 2069 6e74 0a20 2020 2020 2020 2020  x: int.         
-00004e50: 2020 202e 2e2e 2020 2020 2079 3a20 696e     ...     y: in
-00004e60: 740a 2020 2020 2020 2020 2020 2020 2e2e  t.            ..
-00004e70: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00004e80: 3e20 7061 7273 6572 203d 2079 6170 782e  > parser = yapx.
-00004e90: 4172 6775 6d65 6e74 5061 7273 6572 2829  ArgumentParser()
-00004ea0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
-00004eb0: 2070 6172 7365 722e 6164 645f 6172 6775   parser.add_argu
-00004ec0: 6d65 6e74 7328 4164 644e 756d 7329 0a20  ments(AddNums). 
-00004ed0: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
-00004ee0: 6172 7365 6420 3d20 7061 7273 6572 2e70  arsed = parser.p
-00004ef0: 6172 7365 5f61 7267 735f 746f 5f6d 6f64  arse_args_to_mod
-00004f00: 656c 285b 272d 7827 2c20 2731 272c 2027  el(['-x', '1', '
-00004f10: 2d79 272c 2027 3227 5d29 0a20 2020 2020  -y', '2']).     
-00004f20: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-00004f30: 2020 2020 2020 203e 3e3e 2028 7061 7273         >>> (pars
-00004f40: 6564 2e78 2c20 7061 7273 6564 2e79 290a  ed.x, parsed.y).
-00004f50: 2020 2020 2020 2020 2020 2020 2831 2c20              (1, 
-00004f60: 3229 0a0a 2020 2020 2020 2020 72fe 0000  2)..        r...
-00004f70: 0029 0272 f700 0000 72ff 0000 0029 0572  .).r....r....).r
-00004f80: 7600 0000 7250 0000 0072 8d00 0000 72fd  v...rP...r....r.
-00004f90: 0000 0072 0001 0000 7253 0000 0072 5300  ...r....rS...rS.
-00004fa0: 0000 7257 0000 00da 1370 6172 7365 5f61  ..rW.....parse_a
-00004fb0: 7267 735f 746f 5f6d 6f64 656c 9503 0000  rgs_to_model....
-00004fc0: 730c 0000 000a 1e04 0102 0102 0102 0106  s...............
-00004fd0: fd7a 2241 7267 756d 656e 7450 6172 7365  .z"ArgumentParse
-00004fe0: 722e 7061 7273 655f 6172 6773 5f74 6f5f  r.parse_args_to_
-00004ff0: 6d6f 6465 6c63 0400 0000 0000 0000 0000  modelc..........
-00005000: 0000 0800 0000 0a00 0000 4300 0000 73aa  ..........C...s.
-00005010: 0000 0074 007c 0183 017d 047c 0273 107c  ...t.|...}.|.s.|
-00005020: 04a0 017c 006a 02a1 017d 027c 0273 1074  ...|.j...}.|.s.t
-00005030: 0382 017c 006a 047c 047c 0264 018d 027d  ...|.j.|.|.d...}
-00005040: 0574 0572 4e7c 0373 4e7a 0d74 0074 067c  .t.rN|.sNz.t.t.|
-00005050: 0283 0164 0569 007c 05a4 018e 0183 017d  ...d.i.|.......}
-00005060: 0557 006e 2504 0074 0779 4d01 007d 0601  .W.n%..t.yM..}..
-00005070: 007a 1964 0264 02a0 0864 0364 0484 007c  .z.d.d...d.d...|
-00005080: 06a0 09a1 0044 0083 01a1 0117 007d 077c  .....D.......}.|
-00005090: 00a0 0a7c 07a1 0101 0057 0059 0064 007d  ...|.....W.Y.d.}
-000050a0: 067e 066e 0564 007d 067e 0677 0177 007c  .~.n.d.}.~.w.w.|
-000050b0: 0264 0569 007c 05a4 018e 0153 0029 064e  .d.i.|.....S.).N
-000050c0: a902 da09 6172 6773 5f64 6963 7472 8d00  ....args_dictr..
-000050d0: 0000 727b 0000 0063 0100 0000 0000 0000  ..r{...c........
-000050e0: 0000 0000 0200 0000 0600 0000 7300 0000  ............s...
-000050f0: 732e 0000 0081 007c 005d 127d 0164 007c  s......|.].}.d.|
-00005100: 0164 0119 0064 0219 009b 0064 037c 0164  .d...d.....d.|.d
-00005110: 0419 009b 0064 059d 0556 0001 0071 0264  .....d...V...q.d
-00005120: 0653 0029 077a 1845 7272 6f72 2070 6172  .S.).z.Error par
-00005130: 7369 6e67 2061 7267 756d 656e 7420 60da  sing argument `.
-00005140: 036c 6f63 7201 0000 007a 0360 3b20 da03  .locr....z.`; ..
-00005150: 6d73 6772 ab00 0000 4e72 5300 0000 7254  msgr....NrS...rT
-00005160: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
-00005170: 0000 da09 3c67 656e 6578 7072 3ed3 0300  ....<genexpr>...
-00005180: 0073 0a00 0000 0280 0400 0202 1cff 0aff  .s..............
-00005190: 7a36 4172 6775 6d65 6e74 5061 7273 6572  z6ArgumentParser
-000051a0: 2e5f 7061 7273 655f 6172 6773 5f74 6f5f  ._parse_args_to_
-000051b0: 6d6f 6465 6c2e 3c6c 6f63 616c 733e 2e3c  model.<locals>.<
-000051c0: 6765 6e65 7870 723e 7253 0000 0029 0b72  genexpr>rS...).r
-000051d0: f400 0000 72a9 0000 0072 4600 0000 7226  ....r....rF...r&
-000051e0: 0000 00da 165f 756e 696f 6e5f 6172 6773  ....._union_args
-000051f0: 5f77 6974 685f 6d6f 6465 6c72 3500 0000  _with_modelr5...
-00005200: 7233 0000 0072 2e00 0000 72d9 0000 00da  r3...r....r.....
-00005210: 0665 7272 6f72 7372 8000 0000 2908 7276  .errorsr....).rv
-00005220: 0000 0072 5000 0000 728d 0000 0072 fd00  ...rP...r....r..
-00005230: 0000 7200 0100 005a 0a61 7267 735f 756e  ..r....Z.args_un
-00005240: 696f 6e72 fa00 0000 72dc 0000 0072 5300  ionr....r....rS.
-00005250: 0000 7253 0000 0072 5700 0000 72ff 0000  ..rS...rW...r...
-00005260: 00ba 0300 0073 2c00 0000 0806 0402 0c01  .....s,.........
-00005270: 0401 0401 0402 0201 0201 06fe 0805 0202  ................
-00005280: 0201 1001 08ff 0e03 0c01 0602 0afe 1604  ................
-00005290: 0880 02fb 0e07 7a23 4172 6775 6d65 6e74  ......z#Argument
-000052a0: 5061 7273 6572 2e5f 7061 7273 655f 6172  Parser._parse_ar
-000052b0: 6773 5f74 6f5f 6d6f 6465 6c72 0501 0000  gs_to_modelr....
-000052c0: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-000052d0: 0003 0000 0003 0000 0073 1600 0000 8700  .........s......
-000052e0: 6601 6401 6402 8408 7c00 a000 a100 4400  f.d.d...|.....D.
-000052f0: 8301 5300 2903 4e63 0100 0000 0000 0000  ..S.).Nc........
-00005300: 0000 0000 0300 0000 0400 0000 1300 0000  ................
-00005310: 7320 0000 0069 007c 005d 0c5c 027d 017d  s ...i.|.].\.}.}
-00005320: 027c 0188 006a 0076 0072 027c 017c 0293  .|...j.v.r.|.|..
-00005330: 0271 0253 0072 5300 0000 72a0 0000 00a9  .q.S.rS...r.....
-00005340: 0372 5500 0000 72de 0000 00da 0176 7292  .rU...r......vr.
-00005350: 0000 0072 5300 0000 7257 0000 00da 0a3c  ...rS...rW.....<
-00005360: 6469 6374 636f 6d70 3ee0 0300 0072 6100  dictcomp>....ra.
-00005370: 0000 7a39 4172 6775 6d65 6e74 5061 7273  ..z9ArgumentPars
-00005380: 6572 2e5f 756e 696f 6e5f 6172 6773 5f77  er._union_args_w
-00005390: 6974 685f 6d6f 6465 6c2e 3c6c 6f63 616c  ith_model.<local
-000053a0: 733e 2e3c 6469 6374 636f 6d70 3e29 0172  s>.<dictcomp>).r
-000053b0: 8a00 0000 7204 0100 0072 5300 0000 7292  ....r....rS...r.
-000053c0: 0000 0072 5700 0000 7209 0100 00db 0300  ...rW...r.......
-000053d0: 0073 0200 0000 1605 7a25 4172 6775 6d65  .s......z%Argume
-000053e0: 6e74 5061 7273 6572 2e5f 756e 696f 6e5f  ntParser._union_
-000053f0: 6172 6773 5f77 6974 685f 6d6f 6465 6c63  args_with_modelc
-00005400: 0200 0000 0000 0000 0000 0000 0600 0000  ................
-00005410: 0400 0000 4300 0000 7380 0000 0064 007d  ....C...s....d.}
-00005420: 027c 016a 0072 157c 016a 00a0 017c 016a  .|.j.r.|.j...|.j
-00005430: 0264 0117 00a1 0173 157c 016a 00a0 03a1  .d.....s.|.j....
-00005440: 00a0 04a1 007d 027c 0273 1964 0053 0064  .....}.|.s.d.S.d
-00005450: 027d 0374 057c 0283 0144 005d 0c5c 027d  .}.t.|...D.].\.}
-00005460: 047d 057c 05a0 03a1 0073 2b7c 047d 0301  .}.|.....s+|.}..
-00005470: 006e 0171 1f7c 0364 026b 0472 367c 0264  .n.q.|.d.k.r6|.d
-00005480: 007c 0385 0219 007d 0264 03a0 0664 0464  .|.....}.d...d.d
-00005490: 0584 007c 0244 0083 01a1 0153 0029 064e  ...|.D.....S.).N
-000054a0: fa01 2872 0100 0000 727b 0000 0063 0100  ..(r....r{...c..
-000054b0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
-000054c0: 0000 7300 0000 7318 0000 0081 007c 005d  ..s...s......|.]
-000054d0: 077d 017c 01a0 00a1 0056 0001 0071 0264  .}.|.....V...q.d
-000054e0: 0053 0072 5c00 0000 2901 da05 7374 7269  .S.r\...)...stri
-000054f0: 7072 5400 0000 7253 0000 0072 5300 0000  prT...rS...rS...
-00005500: 7257 0000 0072 0801 0000 fa03 0000 7304  rW...r........s.
-00005510: 0000 0002 8016 007a 4141 7267 756d 656e  .......zAArgumen
-00005520: 7450 6172 7365 722e 5f67 6574 5f64 6573  tParser._get_des
-00005530: 6372 6970 7469 6f6e 5f66 726f 6d5f 646f  cription_from_do
-00005540: 6373 7472 696e 672e 3c6c 6f63 616c 733e  cstring.<locals>
-00005550: 2e3c 6765 6e65 7870 723e 2907 da07 5f5f  .<genexpr>)...__
-00005560: 646f 635f 5f72 6000 0000 7294 0000 0072  doc__r`...r....r
-00005570: 0f01 0000 7298 0000 00da 0965 6e75 6d65  ....r......enume
-00005580: 7261 7465 72d9 0000 0029 0672 a600 0000  rater....).r....
-00005590: 728d 0000 005a 1164 6573 6372 6970 7469  r....Z.descripti
-000055a0: 6f6e 5f6c 696e 6573 5a12 7465 7874 5f62  on_linesZ.text_b
-000055b0: 6c6f 636b 5f65 6e64 735f 6174 da01 69da  lock_ends_at..i.
-000055c0: 046c 696e 6572 5300 0000 7253 0000 0072  .linerS...rS...r
-000055d0: 5700 0000 7297 0000 00e2 0300 0073 2000  W...r........s .
-000055e0: 0000 0405 0c02 0801 04ff 0e03 0402 0401  ................
-000055f0: 0402 1001 0801 0401 0401 02fe 0804 0c01  ................
-00005600: 1402 7a2e 4172 6775 6d65 6e74 5061 7273  ..z.ArgumentPars
-00005610: 6572 2e5f 6765 745f 6465 7363 7269 7074  er._get_descript
-00005620: 696f 6e5f 6672 6f6d 5f64 6f63 7374 7269  ion_from_docstri
-00005630: 6e67 6303 0000 0000 0000 0000 0000 0004  ngc.............
-00005640: 0000 0003 0000 0043 0000 0073 1c00 0000  .......C...s....
-00005650: 7c00 a000 7c02 a101 7d03 7c03 720c 7c03  |...|...}.|.r.|.
-00005660: 7c01 5f01 6400 5300 6400 5300 725c 0000  |._.d.S.d.S.r\..
-00005670: 0029 0272 9700 0000 7249 0000 0029 0472  .).r....rI...).r
-00005680: a600 0000 7266 0000 0072 8d00 0000 7249  ....rf...r....rI
-00005690: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
-000056a0: 0000 da1f 5f73 6574 5f64 6573 6372 6970  ...._set_descrip
-000056b0: 7469 6f6e 5f66 726f 6d5f 646f 6373 7472  tion_from_docstr
-000056c0: 696e 67fc 0300 0073 0800 0000 0a06 0402  ing....s........
-000056d0: 0a01 04ff 7a2e 4172 6775 6d65 6e74 5061  ....z.ArgumentPa
-000056e0: 7273 6572 2e5f 7365 745f 6465 7363 7269  rser._set_descri
-000056f0: 7074 696f 6e5f 6672 6f6d 5f64 6f63 7374  ption_from_docst
-00005700: 7269 6e67 da0b 6c69 6e6b 6564 5f66 756e  ring..linked_fun
-00005710: 63da 0b72 656c 6179 5f76 616c 7565 6307  c..relay_valuec.
-00005720: 0000 0000 0000 0000 0000 0017 0000 0007  ................
-00005730: 0000 0003 0000 0073 e601 0000 6700 7d07  .......s....g.}.
-00005740: 6900 7d08 6401 7d09 6401 7d0a 6401 7d0b  i.}.d.}.d.}.d.}.
-00005750: 6401 7d0c 6401 7d0d 7400 7c02 8301 6a01  d.}.d.}.t.|...j.
-00005760: a002 a100 4400 5d43 7d0e 7403 7c0e 8301  ....D.]C}.t.|...
-00005770: a004 6402 a101 7221 6403 7d0c 7115 7403  ..d...r!d.}.q.t.
-00005780: 7c0e 8301 a004 6404 a101 722b 6403 7d0a  |.....d...r+d.}.
-00005790: 7115 7c0e 6a05 6405 6b02 7233 6403 7d0b  q.|.j.d.k.r3d.}.
-000057a0: 7115 7c0e 6a05 6406 6b02 723b 6403 7d0d  q.|.j.d.k.r;d.}.
-000057b0: 7115 7c0e 6a05 6407 6b02 7245 7c03 7c08  q.|.j.d.k.rE|.|.
-000057c0: 6407 3c00 7115 7c0e 6a05 6408 6b02 724f  d.<.q.|.j.d.k.rO
-000057d0: 7c06 7c08 6408 3c00 7115 7c0e 6a05 6409  |.|.d.<.q.|.j.d.
-000057e0: 6b02 7258 6403 7c08 6409 3c00 7115 7c0a  k.rXd.|.d.<.q.|.
-000057f0: 7060 7c0c 7060 7c0b 7060 7c0d 7d09 7c09  p`|.p`|.p`|.}.|.
-00005800: 7373 7c05 7273 7406 640a 640b 8400 7400  ss|.rst.d.d...t.
-00005810: 7c05 8301 6a01 a002 a100 4400 8301 8301  |...j.....D.....
-00005820: 7d09 7c04 7379 7407 7c02 8301 7d04 7c09  }.|.syt.|...}.|.
-00005830: 72e1 7c01 6a08 7c03 7c04 640c 8d02 5c02  r.|.j.|.|.d...\.
-00005840: 7d0f 7d10 7c0c 7388 7c0d 72d6 6900 8900  }.}.|.s.|.r.i...
-00005850: 7c00 8300 7d11 7c10 4400 5d24 7d12 7c12  |...}.|.D.]$}.|.
-00005860: a004 640d a101 72b3 7c12 6a09 640e 640f  ..d...r.|.j.d.d.
-00005870: 6410 8d02 6411 1900 7d13 7c13 a00a 640d  d...d...}.|...d.
-00005880: a101 7d14 7c14 72b3 7c11 6a0b 7c13 6412  ..}.|.r.|.j.|.d.
-00005890: 6400 6401 6413 8d04 0100 7c13 8800 7c14  d.d.d.....|...|.
-000058a0: 3c00 718f 7c11 6a0c 7c10 6414 8d01 5c02  <.q.|.j.|.d...\.
-000058b0: 7d15 7d10 8700 6601 6415 6416 8408 740d  }.}...f.d.d...t.
-000058c0: 7c15 8301 a00e a100 4400 8301 7d16 7c0c  |.......D...}.|.
-000058d0: 72d0 7c08 a00f 7c16 a101 0100 7c0d 72d6  r.|...|.....|.r.
-000058e0: 7c16 7c08 6406 3c00 7c0a 72da 7c10 7d07  |.|.d.<.|.r.|.}.
-000058f0: 7c0b 72e0 7c10 7c08 6405 3c00 6e07 7c01  |.r.|.|.d.<.n.|.
-00005900: 6a10 7c03 7c04 640c 8d02 7d0f 7c02 7c07  j.|.|.d...}.|.|.
-00005910: 6900 740d 7c0f 8301 a401 7c08 a401 8e01  i.t.|.....|.....
-00005920: 5300 2917 4e46 7a02 2a2a 54da 012a da0b  S.).NFz.**T..*..
-00005930: 5f65 7874 7261 5f61 7267 73da 0d5f 6578  _extra_args.._ex
-00005940: 7472 615f 6b77 6172 6773 5a09 5f61 6c6c  tra_kwargsZ._all
-00005950: 5f61 7267 735a 0c5f 7265 6c61 795f 7661  _argsZ._relay_va
-00005960: 6c75 655a 105f 6361 6c6c 6564 5f66 726f  lueZ._called_fro
-00005970: 6d5f 636c 6963 0100 0000 0000 0000 0000  m_clic..........
-00005980: 0000 0200 0000 0400 0000 7300 0000 7328  ..........s...s(
-00005990: 0000 0081 007c 005d 0f7d 0174 007c 0183  .....|.].}.t.|..
-000059a0: 01a0 0164 00a1 0170 0f7c 016a 0264 0176  ...d...p.|.j.d.v
-000059b0: 0056 0001 0071 0264 0253 0029 0372 1701  .V...q.d.S.).r..
-000059c0: 0000 2902 7218 0100 0072 1901 0000 4e29  ..).r....r....N)
-000059d0: 0372 6d00 0000 7260 0000 0072 9000 0000  .rm...r`...r....
-000059e0: 2902 7255 0000 00da 0170 7253 0000 0072  ).rU.....prS...r
-000059f0: 5300 0000 7257 0000 0072 0801 0000 3104  S...rW...r....1.
-00005a00: 0000 730a 0000 0002 8004 0002 0216 ff0a  ..s.............
-00005a10: ff7a 2b41 7267 756d 656e 7450 6172 7365  .z+ArgumentParse
-00005a20: 722e 5f72 756e 5f66 756e 632e 3c6c 6f63  r._run_func.<loc
-00005a30: 616c 733e 2e3c 6765 6e65 7870 723e 2902  als>.<genexpr>).
-00005a40: 7250 0000 0072 8d00 0000 7265 0000 0072  rP...r....re...r
-00005a50: 5b00 0000 7217 0000 0072 ac00 0000 7201  [...r....r....r.
-00005a60: 0000 0072 b800 0000 2903 72b7 0000 0072  ...r....).r....r
-00005a70: 6300 0000 72b6 0000 0029 0172 5000 0000  c...r....).rP...
-00005a80: 6301 0000 0000 0000 0000 0000 0003 0000  c...............
-00005a90: 0004 0000 0013 0000 0073 1a00 0000 6900  .........s....i.
-00005aa0: 7c00 5d09 5c02 7d01 7d02 8800 7c01 1900  |.].\.}.}...|...
-00005ab0: 7c02 9302 7102 5300 7253 0000 0072 5300  |...q.S.rS...rS.
-00005ac0: 0000 720b 0100 00a9 015a 1075 6e6b 6e6f  ..r......Z.unkno
-00005ad0: 776e 5f6e 616d 655f 6d61 7072 5300 0000  wn_name_maprS...
-00005ae0: 7257 0000 0072 0d01 0000 5504 0000 7306  rW...r....U...s.
-00005af0: 0000 0006 000e 0106 ff7a 2c41 7267 756d  .........z,Argum
-00005b00: 656e 7450 6172 7365 722e 5f72 756e 5f66  entParser._run_f
-00005b10: 756e 632e 3c6c 6f63 616c 733e 2e3c 6469  unc.<locals>.<di
-00005b20: 6374 636f 6d70 3e29 1172 0900 0000 da0a  ctcomp>).r......
-00005b30: 7061 7261 6d65 7465 7273 72bd 0000 0072  parametersr....r
-00005b40: 6d00 0000 7260 0000 0072 9000 0000 da03  m...r`...r......
-00005b50: 616e 7972 2500 0000 7202 0100 00da 0573  anyr%...r......s
-00005b60: 706c 6974 da06 6c73 7472 6970 726e 0000  plit..lstriprn..
-00005b70: 0072 fb00 0000 72f4 0000 0072 8a00 0000  .r....r....r....
-00005b80: da06 7570 6461 7465 7203 0100 0029 1772  ..updater....).r
-00005b90: a600 0000 7266 0000 0072 9b00 0000 7250  ....rf...r....rP
-00005ba0: 0000 0072 8d00 0000 7215 0100 0072 1601  ...r....r....r..
-00005bb0: 0000 5a09 6675 6e63 5f61 7267 735a 0b66  ..Z.func_argsZ.f
-00005bc0: 756e 635f 6b77 6172 6773 5a0d 6578 7472  unc_kwargsZ.extr
-00005bd0: 615f 6172 6773 5f6f 6b5a 0c61 6363 6570  a_args_okZ.accep
-00005be0: 7473 5f61 7267 735a 1261 6363 6570 7473  ts_argsZ.accepts
-00005bf0: 5f65 7874 7261 5f61 7267 735a 0e61 6363  _extra_argsZ.acc
-00005c00: 6570 7473 5f6b 7761 7267 735a 1461 6363  epts_kwargsZ.acc
-00005c10: 6570 7473 5f65 7874 7261 5f6b 7761 7267  epts_extra_kwarg
-00005c20: 7372 1a01 0000 5a0a 6d6f 6465 6c5f 696e  sr....Z.model_in
-00005c30: 7374 7201 0100 005a 0e75 6e6b 6e6f 776e  str....Z.unknown
-00005c40: 5f70 6172 7365 7272 5600 0000 5a06 785f  _parserrV...Z.x_
-00005c50: 666c 6167 5a0b 785f 666c 6167 5f62 6172  flagZ.x_flag_bar
-00005c60: 655a 0e70 6172 7365 645f 756e 6b6e 6f77  eZ.parsed_unknow
-00005c70: 6e5a 0c65 7874 7261 5f6b 7761 7267 7372  nZ.extra_kwargsr
-00005c80: 5300 0000 721b 0100 0072 5700 0000 da09  S...r....rW.....
-00005c90: 5f72 756e 5f66 756e 6307 0400 0073 9000  _run_func....s..
-00005ca0: 0000 040a 0401 0402 0402 0401 0402 0401  ................
-00005cb0: 1202 0e01 0601 0e01 0601 0a01 0601 0a01  ................
-00005cc0: 0601 0a01 0a01 0a01 0a01 0a01 0801 0280  ................
-00005cd0: 0e03 02ff 0804 0801 0c02 08fe 0405 0801  ................
-00005ce0: 0403 0402 0201 0201 0afe 0805 0401 0601  ................
-00005cf0: 0801 0a01 1201 0a01 0401 0401 0201 0201  ................
-00005d00: 0201 0201 06fc 0806 0280 0402 0201 0aff  ................
-00005d10: 0a04 0a01 06ff 0403 0a01 0401 0801 0402  ................
-00005d20: 0401 0402 0801 0280 0403 0201 0201 06fe  ................
-00005d30: 1605 7a18 4172 6775 6d65 6e74 5061 7273  ..z.ArgumentPars
-00005d40: 6572 2e5f 7275 6e5f 6675 6e63 da07 636f  er._run_func..co
-00005d50: 6d6d 616e 64da 0b73 7562 636f 6d6d 616e  mmand..subcomman
-00005d60: 6473 da11 6e61 6d65 645f 7375 6263 6f6d  ds..named_subcom
-00005d70: 6d61 6e64 7363 0400 0000 0000 0000 0000  mandsc..........
-00005d80: 0000 0900 0000 0b00 0000 4b00 0000 73d2  ..........K...s.
-00005d90: 0000 007c 0064 0369 007c 04a4 018e 017d  ...|.d.i.|.....}
-00005da0: 057c 0172 2e74 007c 0183 017d 067c 006a  .|.r.t.|...}.|.j
-00005db0: 017c 057c 0664 018d 0201 007c 05a0 027c  .|.|.d.....|...|
-00005dc0: 06a1 0101 007c 056a 0364 0369 007c 006a  .....|.j.d.i.|.j
-00005dd0: 047c 017c 006a 057c 067c 006a 067c 017c  .|.|.j.|.|.j.|.|
-00005de0: 006a 077c 0669 04a4 018e 0101 006e 147c  .j.|.i.......n.|
-00005df0: 056a 0364 0369 007c 006a 0564 007c 006a  .j.d.i.|.j.d.|.j
-00005e00: 0464 007c 006a 0764 007c 006a 0664 0069  .d.|.j.d.|.j.d.i
-00005e10: 04a4 018e 0101 007c 0272 5574 087c 0283  .......|.rUt.|..
-00005e20: 0172 4b7c 0267 017d 027c 0244 005d 077d  .rK|.g.}.|.D.].}
-00005e30: 077c 05a0 097c 07a1 0101 0071 4d7c 0372  .|...|.....qM|.r
-00005e40: 677c 03a0 0aa1 0044 005d 0b5c 027d 087d  g|.....D.].\.}.}
-00005e50: 077c 056a 097c 077c 0864 028d 0201 0071  .|.j.|.|.d.....q
-00005e60: 5b7c 0553 0029 044e 2902 7266 0000 0072  [|.S.).N).rf...r
-00005e70: 8d00 0000 72b0 0000 0072 5300 0000 290b  ....r....rS...).
-00005e80: 7225 0000 0072 1401 0000 728f 0000 0072  r%...r....r....r
-00005e90: 9c00 0000 7242 0000 0072 4300 0000 7245  ....rB...rC...rE
-00005ea0: 0000 0072 4600 0000 da08 6361 6c6c 6162  ...rF.....callab
-00005eb0: 6c65 729d 0000 0072 8a00 0000 2909 72a6  ler....r....).r.
-00005ec0: 0000 0072 2201 0000 7223 0100 0072 2401  ...r"...r#...r$.
-00005ed0: 0000 7251 0000 0072 6600 0000 5a0e 726f  ..rQ...rf...Z.ro
-00005ee0: 6f74 5f61 7267 5f6d 6f64 656c 7256 0000  ot_arg_modelrV..
-00005ef0: 0072 9000 0000 7253 0000 0072 5300 0000  .r....rS...rS...
-00005f00: 7257 0000 00da 0d5f 6275 696c 645f 7061  rW....._build_pa
-00005f10: 7273 6572 6b04 0000 733e 0000 000e 0804  rserk...s>......
-00005f20: 0208 0104 0102 0102 0106 fe0a 0408 0106  ................
-00005f30: 0206 0106 0106 0102 fc08 ff08 0906 0206  ................
-00005f40: 0106 0106 0102 fc06 ff04 0908 0106 0108  ................
-00005f50: 010c 0104 0210 0110 0104 027a 1c41 7267  ...........z.Arg
-00005f60: 756d 656e 7450 6172 7365 722e 5f62 7569  umentParser._bui
-00005f70: 6c64 5f70 6172 7365 7229 0272 5000 0000  ld_parser).rP...
-00005f80: da0c 6465 6661 756c 745f 6172 6773 da0b  ..default_args..
-00005f90: 7061 7273 6572 5f61 7267 7372 2701 0000  parser_argsr'...
-00005fa0: da0d 7061 7273 6572 5f6b 7761 7267 7363  ..parser_kwargsc
-00005fb0: 0100 0000 0000 0000 0200 0000 1100 0000  ................
-00005fc0: 0900 0000 4f00 0000 7338 0100 007c 006a  ....O...s8...|.j
-00005fd0: 007c 0369 007c 04a4 018e 017d 057c 0164  .|.i.|.....}.|.d
-00005fe0: 0175 0072 1374 016a 0264 0264 0185 0219  .u.r.t.j.d.d....
-00005ff0: 007d 017c 0173 197c 0272 197c 027d 017c  .}.|.s.|.r.|.}.|
-00006000: 05a0 037c 01a1 015c 027d 067d 0774 047c  ...|...\.}.}.t.|
-00006010: 0683 017d 087c 08a0 057c 006a 06a1 017d  ...}.|...|.j...}
-00006020: 097c 08a0 057c 006a 07a1 017d 0a7c 08a0  .|...|.j...}.|..
-00006030: 057c 006a 08a1 017d 0b7c 08a0 057c 006a  .|.j...}.|...|.j
-00006040: 09a1 017d 0c7c 08a0 057c 006a 0aa1 017d  ...}.|...|.j...}
-00006050: 0d64 017d 0e64 017d 0f7c 0972 527c 006a  .d.}.d.}.|.rR|.j
-00006060: 0b7c 057c 097c 0a7c 0c7c 0164 038d 057d  .|.|.|.|.|.d...}
-00006070: 0f74 0c7c 0f74 0d83 0272 697a 0674 0e7c  .t.|.t...riz.t.|
-00006080: 0f83 017d 0e57 006e 0d04 0074 0f79 6801  ...}.W.n...t.yh.
-00006090: 0001 0001 007c 0f7d 0e59 006e 0377 007c  .....|.}.Y.n.w.|
-000060a0: 0f7d 0e7a 207c 0b72 7b7c 0c72 7b7c 006a  .}.z |.r{|.r{|.j
-000060b0: 0b7c 057c 0c7c 0d7c 017c 097c 0e64 048d  .|.|.|.|.|.|.d..
-000060c0: 067d 0e57 0074 0c7c 0f74 0d83 0272 8a7c  .}.W.t.|.t...r.|
-000060d0: 0f44 005d 067d 107c 0c73 897c 107d 0e71  .D.].}.|.s.|.}.q
-000060e0: 837c 0e53 0074 0c7c 0f74 0d83 0272 9a7c  .|.S.t.|.t...r.|
-000060f0: 0f44 005d 077d 107c 0c73 997c 107d 0e71  .D.].}.|.s.|.}.q
-00006100: 9377 0077 0029 0561 2d03 0000 5573 6520  .w.w.).a-...Use 
-00006110: 6769 7665 6e20 6675 6e63 7469 6f6e 7320  given functions 
-00006120: 746f 2063 6f6e 7374 7275 6374 2061 2043  to construct a C
-00006130: 4c49 2c20 7061 7273 6520 7468 6520 6172  LI, parse the ar
-00006140: 6773 2c20 616e 6420 696e 766f 6b65 2074  gs, and invoke t
-00006150: 6865 2061 7070 726f 7072 6961 7465 2063  he appropriate c
-00006160: 6f6d 6d61 6e64 2e0a 0a20 2020 2020 2020  ommand...       
-00006170: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00006180: 2020 202a 7061 7273 6572 5f61 7267 733a     *parser_args:
-00006190: 0a20 2020 2020 2020 2020 2020 2061 7267  .            arg
-000061a0: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
-000061b0: 6566 6175 6c74 5f61 7267 733a 0a20 2020  efault_args:.   
-000061c0: 2020 2020 2020 2020 202a 2a70 6172 7365           **parse
-000061d0: 725f 6b77 6172 6773 3a0a 0a0a 2020 2020  r_kwargs:...    
-000061e0: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-000061f0: 2020 2020 2020 2020 2020 3e3e 3e20 696d            >>> im
-00006200: 706f 7274 2079 6170 780a 2020 2020 2020  port yapx.      
-00006210: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
-00006220: 2020 2020 2020 3e3e 3e20 6465 6620 7072        >>> def pr
-00006230: 696e 745f 6e75 6d73 282a 6172 6773 293a  int_nums(*args):
-00006240: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00006250: 2020 2020 2070 7269 6e74 2827 4172 6773       print('Args
-00006260: 3a20 272c 202a 6172 6773 290a 2020 2020  : ', *args).    
-00006270: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00006280: 2020 2020 2020 2020 3e3e 3e20 6465 6620          >>> def 
-00006290: 6669 6e64 5f65 7665 6e73 282a 6172 6773  find_evens(*args
-000062a0: 293a 0a20 2020 2020 2020 2020 2020 202e  ):.            .
-000062b0: 2e2e 2020 2020 2072 6574 7572 6e20 5b78  ..     return [x
-000062c0: 2066 6f72 2078 2069 6e20 6172 6773 2069   for x in args i
-000062d0: 6620 696e 7428 7829 2025 2032 203d 3d20  f int(x) % 2 == 
-000062e0: 305d 0a20 2020 2020 2020 2020 2020 202e  0].            .
+00000c90: 047c 0ba4 018e 0101 0064 007c 005f 0264  .|.......d.|._.d
+00000ca0: 037c 006a 035f 047c 0464 0075 0072 2164  .|.j._.|.d.u.r!d
+00000cb0: 0464 0567 027d 047c 0472 3974 057c 0474  .d.g.}.|.r9t.|.t
+00000cc0: 0683 0272 2b7c 0467 017d 047c 006a 0764  ...r+|.g.}.|.j.d
+00000cd0: 0664 0784 007c 0444 0083 0174 0864 0864  .d...|.D...t.d.d
+00000ce0: 099c 028e 0101 0064 0a7c 005f 0974 0a64  .......d.|._.t.d
+00000cf0: 0b64 0c84 0083 017c 005f 0b69 007c 005f  .d.....|._.i.|._
+00000d00: 0c7c 0973 f17c 0472 5a64 0d64 0784 007c  .|.s.|.rZd.d...|
+00000d10: 0444 0083 017d 0c7c 006a 077c 0c74 0d64  .D...}.|.j.|.t.d
+00000d20: 0e64 099c 028e 0101 007c 0564 0075 0072  .d.......|.d.u.r
+00000d30: 6164 0f67 017d 057c 0572 9974 057c 0574  ad.g.}.|.r.t.|.t
+00000d40: 0683 0272 6b7c 0567 017d 057c 006a 0e72  ...rk|.g.}.|.j.r
+00000d50: 8a7c 0273 8a74 0f74 1083 018f 0e01 0074  .|.s.t.t.......t
+00000d60: 117c 006a 0e83 016a 127d 0257 0064 0004  .|.j...j.}.W.d..
+00000d70: 0004 0083 0301 006e 0831 0073 8577 0101  .......n.1.s.w..
+00000d80: 0001 0001 0059 0001 007c 0272 997c 006a  .....Y...|.r.|.j
+00000d90: 077c 0564 1064 117c 029b 009d 0264 1264  .|.d.d.|.....d.d
+00000da0: 139c 038e 0101 007c 0764 0075 0072 a064  .......|.d.u.r.d
+00000db0: 1467 017d 0774 1372 b97c 0772 b974 057c  .g.}.t.r.|.r.t.|
+00000dc0: 0774 0683 0272 ac7c 0767 017d 077c 006a  .t...r.|.g.}.|.j
+00000dd0: 077c 0774 1483 0074 156a 1674 1764 1564  .|.t...t.j.t.d.d
+00000de0: 169c 048e 0101 007c 0664 0075 0072 c064  .......|.d.u.r.d
+00000df0: 1767 017d 067c 0672 f374 1872 f574 057c  .g.}.|.r.t.r.t.|
+00000e00: 0674 0683 0272 cc7c 0667 017d 0674 197c  .t...r.|.g.}.t.|
+00000e10: 0683 0164 186b 0272 e87c 0664 1919 00a0  ...d.k.r.|.d....
+00000e20: 1a64 1aa1 0173 e87c 00a0 1ba1 0001 0074  .d...s.|.......t
+00000e30: 1c7c 007c 0664 1919 0064 1b64 1c8d 0301  .|.|.d...d.d....
+00000e40: 0064 0053 0074 1d7c 007c 0664 1b64 1c8d  .d.S.t.|.|.d.d..
+00000e50: 0301 0064 0053 0064 0053 0064 0053 0064  ...d.S.d.S.d.S.d
+00000e60: 0053 0029 1d4e 4629 0472 4700 0000 7249  .S.).NF).rG...rI
+00000e70: 0000 00da 0861 6464 5f68 656c 7072 4e00  .....add_helprN.
+00000e80: 0000 7a12 6865 6c70 6675 6c20 7061 7261  ..z.helpful para
+00000e90: 6d65 7465 7273 7a02 2d68 7a06 2d2d 6865  metersz.-hz.--he
+00000ea0: 6c70 6301 0000 0000 0000 0000 0000 0002  lpc.............
+00000eb0: 0000 0003 0000 0053 0000 0073 1400 0000  .......S...s....
+00000ec0: 6700 7c00 5d06 7d01 7c01 7202 7c01 9102  g.|.].}.|.r.|...
+00000ed0: 7102 5300 a900 7253 0000 00a9 02da 022e  q.S...rS........
+00000ee0: 30da 0178 7253 0000 0072 5300 0000 fa26  0..xrS...rS....&
+00000ef0: 2f64 726f 6e65 2f73 7263 2f73 7263 2f79  /drone/src/src/y
+00000f00: 6170 782f 6172 6775 6d65 6e74 5f70 6172  apx/argument_par
+00000f10: 7365 722e 7079 da0a 3c6c 6973 7463 6f6d  ser.py..<listcom
+00000f20: 703e 7600 0000 7302 0000 0014 007a 2b41  p>v...s......z+A
+00000f30: 7267 756d 656e 7450 6172 7365 722e 5f5f  rgumentParser.__
+00000f40: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
+00000f50: 3c6c 6973 7463 6f6d 703e 7a17 5368 6f77  <listcomp>z.Show
+00000f60: 2074 6869 7320 6865 6c70 206d 6573 7361   this help messa
+00000f70: 6765 2e29 02da 0661 6374 696f 6eda 0468  ge.)...action..h
+00000f80: 656c 70fa 013d 6300 0000 0000 0000 0000  elp..=c.........
+00000f90: 0000 0000 0000 0002 0000 0053 0000 0073  ...........S...s
+00000fa0: 0800 0000 7400 7401 8301 5300 a901 4e29  ....t.t...S...N)
+00000fb0: 0272 0200 0000 da04 6c69 7374 7253 0000  .r......listrS..
+00000fc0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+00000fd0: da08 3c6c 616d 6264 613e 8000 0000 7302  ..<lambda>....s.
+00000fe0: 0000 0008 007a 2941 7267 756d 656e 7450  .....z)ArgumentP
+00000ff0: 6172 7365 722e 5f5f 696e 6974 5f5f 2e3c  arser.__init__.<
+00001000: 6c6f 6361 6c73 3e2e 3c6c 616d 6264 613e  locals>.<lambda>
+00001010: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001020: 0005 0000 0053 0000 0073 2000 0000 6700  .....S...s ...g.
+00001030: 7c00 5d0c 7d01 7c01 a000 6400 a101 7202  |.].}.|...d...r.
+00001040: 7c01 9b00 6401 9d02 9102 7102 5300 2902  |...d.....q.S.).
+00001050: 7a02 2d2d 7a04 2d61 6c6c a901 da0a 7374  z.--z.-all....st
+00001060: 6172 7473 7769 7468 7254 0000 0072 5300  artswithrT...rS.
+00001070: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
+00001080: 0086 0000 00f3 0200 0000 2000 7a1b 5368  .......... .z.Sh
+00001090: 6f77 2068 656c 7020 666f 7220 616c 6c20  ow help for all 
+000010a0: 636f 6d6d 616e 6473 2e7a 092d 2d76 6572  commands.z.--ver
+000010b0: 7369 6f6e da07 7665 7273 696f 6e7a 0925  sion..versionz.%
+000010c0: 2870 726f 6729 7320 7a20 5368 6f77 2074  (prog)s z Show t
+000010d0: 6865 2070 726f 6772 616d 2076 6572 7369  he program versi
+000010e0: 6f6e 206e 756d 6265 722e 2903 7259 0000  on number.).rY..
+000010f0: 0072 6200 0000 725a 0000 007a 182d 2d70  .rb...rZ...z.--p
+00001100: 7269 6e74 2d73 6865 6c6c 2d63 6f6d 706c  rint-shell-compl
+00001110: 6574 696f 6e7a 1e50 7269 6e74 2073 6865  etionz.Print she
+00001120: 6c6c 2063 6f6d 706c 6574 696f 6e20 7363  ll completion sc
+00001130: 7269 7074 2e29 0472 5900 0000 da07 6465  ript.).rY.....de
+00001140: 6661 756c 74da 0763 686f 6963 6573 725a  fault..choicesrZ
+00001150: 0000 007a 052d 2d74 7569 7217 0000 0072  ...z.--tuir....r
+00001160: 0100 0000 fa01 2d7a 2253 686f 7720 5465  ......-z"Show Te
+00001170: 7874 7561 6c20 5573 6572 2049 6e74 6572  xtual User Inter
+00001180: 6661 6365 2028 5455 4929 2e29 03da 0670  face (TUI).)...p
+00001190: 6172 7365 72da 0e6f 7074 696f 6e5f 7374  arser..option_st
+000011a0: 7269 6e67 7372 5a00 0000 291e da05 7375  ringsrZ...)...su
+000011b0: 7065 72da 085f 5f69 6e69 745f 5fda 125f  per..__init__.._
+000011c0: 7375 6270 6172 7365 7273 5f61 6374 696f  subparsers_actio
+000011d0: 6eda 0a5f 6f70 7469 6f6e 616c 73da 0574  n.._optionals..t
+000011e0: 6974 6c65 da0a 6973 696e 7374 616e 6365  itle..isinstance
+000011f0: da03 7374 72da 0c61 6464 5f61 7267 756d  ..str..add_argum
+00001200: 656e 7472 1b00 0000 da0c 6b76 5f73 6570  entr......kv_sep
+00001210: 6172 6174 6f72 7202 0000 00da 185f 6d75  aratorr......_mu
+00001220: 7475 616c 6c79 5f65 7863 6c75 7369 7665  tually_exclusive
+00001230: 5f61 7267 73da 0a5f 6465 7374 5f74 7970  _args.._dest_typ
+00001240: 6572 1c00 0000 7247 0000 0072 0300 0000  er....rG...r....
+00001250: da09 4578 6365 7074 696f 6e72 1600 0000  ..Exceptionr....
+00001260: 7262 0000 0072 3600 0000 7232 0000 00da  rb...r6...r2....
+00001270: 0861 7267 7061 7273 65da 0853 5550 5052  .argparse..SUPPR
+00001280: 4553 5372 2c00 0000 7237 0000 00da 036c  ESSr,...r7.....l
+00001290: 656e 7260 0000 00da 165f 6765 745f 6f72  enr`....._get_or
+000012a0: 5f61 6464 5f73 7562 7061 7273 6572 7372  _add_subparsersr
+000012b0: 3000 0000 722f 0000 0029 0dda 0473 656c  0...r/...)...sel
+000012c0: 6672 4700 0000 7248 0000 0072 4900 0000  frG...rH...rI...
+000012d0: 724a 0000 0072 4b00 0000 724c 0000 0072  rJ...rK...rL...r
+000012e0: 4d00 0000 724e 0000 0072 4f00 0000 7250  M...rN...rO...rP
+000012f0: 0000 0072 5100 0000 5a0e 6865 6c70 5f61  ...rQ...Z.help_a
+00001300: 6c6c 5f66 6c61 6773 a901 da09 5f5f 636c  ll_flags....__cl
+00001310: 6173 735f 5f72 5300 0000 7257 0000 0072  ass__rS...rW...r
+00001320: 6900 0000 5300 0000 73a0 0000 0006 0e02  i...S...s.......
+00001330: 0102 010a 0102 0102 0104 fb02 0606 fa06  ................
+00001340: 0908 0308 0208 0104 020a 0106 0104 010c  ................
+00001350: 0102 0102 0108 fd06 060a 0504 fd06 0504  ................
+00001360: 0204 010e 0104 0102 0102 0102 0108 fd08  ................
+00001370: 0606 0104 020a 0106 010a 020a 010e 011c  ................
+00001380: ff04 0304 0102 0102 0108 0102 0108 fc08  ................
+00001390: 0706 0108 020a 0106 0104 0202 0104 0104  ................
+000013a0: 0102 0102 0108 fb08 0806 0108 020a 0106  ................
+000013b0: 011a 0208 0102 0102 0106 0102 010a fd02  ................
+000013c0: 0602 0102 0102 010a fd04 c608 2e7a 1741  .............z.A
+000013d0: 7267 756d 656e 7450 6172 7365 722e 5f5f  rgumentParser.__
+000013e0: 696e 6974 5f5f da07 6d65 7373 6167 6563  init__..messagec
+000013f0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+00001400: 0600 0000 4300 0000 7324 0000 007c 00a0  ....C...s$...|..
+00001410: 0074 016a 02a1 0101 007c 00a0 0364 0164  .t.j.....|...d.d
+00001420: 027c 019b 0064 039d 03a1 0201 0064 0053  .|...d.......d.S
+00001430: 0029 044e e902 0000 007a 0765 7272 6f72  .).N.....z.error
+00001440: 3a20 da01 0a29 04da 0b70 7269 6e74 5f75  : ...)...print_u
+00001450: 7361 6765 da03 7379 73da 0673 7464 6572  sage..sys..stder
+00001460: 72da 0465 7869 7429 0272 7800 0000 727b  r..exit).rx...r{
+00001470: 0000 0072 5300 0000 7253 0000 0072 5700  ...rS...rS...rW.
+00001480: 0000 da05 6572 726f 72c4 0000 0073 0400  ....error....s..
+00001490: 0000 0c01 1801 7a14 4172 6775 6d65 6e74  ......z.Argument
+000014a0: 5061 7273 6572 2e65 7272 6f72 da04 6669  Parser.error..fi
+000014b0: 6c65 da10 696e 636c 7564 655f 636f 6d6d  le..include_comm
+000014c0: 616e 6473 da06 7265 7475 726e 6303 0000  ands..returnc...
+000014d0: 0000 0000 0000 0000 0008 0000 0005 0000  ................
+000014e0: 0003 0000 0073 9c00 0000 6401 7d03 7c03  .....s....d.}.|.
+000014f0: 6402 1400 6403 1700 7d04 7400 8300 0100  d...d...}.t.....
+00001500: 7400 7c04 8301 0100 7400 6404 7c00 6a01  t.|.....t.d.|.j.
+00001510: 9b00 9d02 8301 0100 7400 7c04 8301 0100  ........t.|.....
+00001520: 7c00 6a02 7d05 7403 6a04 7c00 5f02 7405  |.j.}.t.j.|._.t.
+00001530: 8300 a006 7c01 a101 0100 7c02 7249 7c00  ....|.....|.rI|.
+00001540: 6a07 7249 7c00 6a08 6405 7500 7237 7c00  j.rI|.j.d.u.r7|.
+00001550: a009 a100 7c00 5f08 7c00 6a08 6a0a a00b  ....|._.|.j.j...
+00001560: a100 4400 5d0b 5c02 7d06 7d07 7c07 6a06  ..D.].\.}.}.|.j.
+00001570: 7c01 7c02 6406 8d02 0100 713d 7c05 7c00  |.|.d.....q=|.|.
+00001580: 5f02 6405 5300 2907 6118 0200 0050 7269  _.d.S.).a....Pri
+00001590: 6e74 2043 4c49 2068 656c 702e 0a0a 2020  nt CLI help...  
+000015a0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000015b0: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+000015c0: 636f 6d6d 616e 6473 3a20 6966 2054 7275  commands: if Tru
+000015d0: 652c 2061 6c73 6f20 7072 696e 7420 6865  e, also print he
+000015e0: 6c70 2066 6f72 2065 6163 6820 636f 6d6d  lp for each comm
+000015f0: 616e 642e 0a0a 2020 2020 2020 2020 4578  and...        Ex
+00001600: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00001610: 2020 2020 3e3e 3e20 696d 706f 7274 2079      >>> import y
+00001620: 6170 780a 2020 2020 2020 2020 2020 2020  apx.            
+00001630: 3e3e 3e20 6672 6f6d 2064 6174 6163 6c61  >>> from datacla
+00001640: 7373 6573 2069 6d70 6f72 7420 6461 7461  sses import data
+00001650: 636c 6173 730a 2020 2020 2020 2020 2020  class.          
+00001660: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00001670: 2020 3e3e 3e20 4064 6174 6163 6c61 7373    >>> @dataclass
+00001680: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00001690: 2063 6c61 7373 2041 6464 4e75 6d73 3a0a   class AddNums:.
+000016a0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+000016b0: 2020 2020 783a 2069 6e74 0a20 2020 2020      x: int.     
+000016c0: 2020 2020 2020 202e 2e2e 2020 2020 2079         ...     y
+000016d0: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
+000016e0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+000016f0: 2020 3e3e 3e20 7061 7273 6572 203d 2079    >>> parser = y
+00001700: 6170 782e 4172 6775 6d65 6e74 5061 7273  apx.ArgumentPars
+00001710: 6572 2829 0a20 2020 2020 2020 2020 2020  er().           
+00001720: 203e 3e3e 2070 6172 7365 722e 6164 645f   >>> parser.add_
+00001730: 6172 6775 6d65 6e74 7328 4164 644e 756d  arguments(AddNum
+00001740: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
+00001750: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
+00001760: 3e3e 2070 6172 7365 722e 7072 696e 745f  >> parser.print_
+00001770: 6865 6c70 2869 6e63 6c75 6465 5f63 6f6d  help(include_com
+00001780: 6d61 6e64 733d 5472 7565 2920 2023 646f  mands=True)  #do
+00001790: 6374 6573 743a 202b 534b 4950 0a20 2020  ctest: +SKIP.   
+000017a0: 2020 2020 20da 015f e950 0000 0072 7d00       .._.P...r}.
+000017b0: 0000 7a02 2420 4e29 0172 8400 0000 290c  ..z.$ N).r....).
+000017c0: da05 7072 696e 7472 4700 0000 da05 7573  ..printrG.....us
+000017d0: 6167 6572 7400 0000 7275 0000 0072 6800  agert...ru...rh.
+000017e0: 0000 da0a 7072 696e 745f 6865 6c70 da0b  ....print_help..
+000017f0: 5f73 7562 7061 7273 6572 7372 6a00 0000  _subparsersrj...
+00001800: da17 5f66 696e 645f 7375 6270 6172 7365  .._find_subparse
+00001810: 7273 5f61 6374 696f 6e72 6400 0000 da05  rs_actionrd.....
+00001820: 6974 656d 7329 0872 7800 0000 7283 0000  items).rx...r...
+00001830: 0072 8400 0000 5a08 7365 705f 6368 6172  .r....Z.sep_char
+00001840: da09 7365 7061 7261 746f 7272 8900 0000  ..separatorr....
+00001850: 5a07 5f63 686f 6963 655a 0973 7562 7061  Z._choiceZ.subpa
+00001860: 7273 6572 7279 0000 0072 5300 0000 7257  rserry...rS...rW
+00001870: 0000 0072 8a00 0000 c800 0000 731e 0000  ...r........s...
+00001880: 0004 180c 0106 0108 0110 0108 0106 0308  ................
+00001890: 010c 020a 020a 010a 0114 0210 010a 027a  ...............z
+000018a0: 1941 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
+000018b0: 7072 696e 745f 6865 6c70 da0a 6172 6773  print_help..args
+000018c0: 5f6d 6f64 656c 2e63 0200 0000 0000 0000  _model.c........
+000018d0: 0000 0000 0200 0000 0400 0000 4300 0000  ............C...
+000018e0: 7310 0000 007c 00a0 007c 007c 01a1 0201  s....|...|.|....
+000018f0: 0064 0153 0029 0261 d605 0000 4164 6420  .d.S.).a....Add 
+00001900: 6172 6775 6d65 6e74 7320 6672 6f6d 2074  arguments from t
+00001910: 6865 2067 6976 656e 2066 756e 6374 696f  he given functio
+00001920: 6e20 6f72 2064 6174 6166 7261 6d65 2e0a  n or dataframe..
+00001930: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+00001940: 2020 2020 2020 2020 2020 2061 7267 735f             args_
+00001950: 6d6f 6465 6c3a 2061 2066 756e 6374 696f  model: a functio
+00001960: 6e20 6f72 2064 6174 6163 6c61 7373 2066  n or dataclass f
+00001970: 726f 6d20 7768 6963 6820 746f 2064 6572  rom which to der
+00001980: 6976 6520 6172 6775 6d65 6e74 732e 0a0a  ive arguments...
+00001990: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+000019a0: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
+000019b0: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
+000019c0: 2020 2020 2020 2020 2020 3e3e 3e20 6672            >>> fr
+000019d0: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
+000019e0: 6d70 6f72 7420 6461 7461 636c 6173 730a  mport dataclass.
+000019f0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00001a00: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00001a10: 4064 6174 6163 6c61 7373 0a20 2020 2020  @dataclass.     
+00001a20: 2020 2020 2020 202e 2e2e 2063 6c61 7373         ... class
+00001a30: 2041 6464 4e75 6d73 3a0a 2020 2020 2020   AddNums:.      
+00001a40: 2020 2020 2020 2e2e 2e20 2020 2020 783a        ...     x:
+00001a50: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00001a60: 202e 2e2e 2020 2020 2079 3a20 696e 740a   ...     y: int.
+00001a70: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00001a80: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00001a90: 7061 7273 6572 203d 2079 6170 782e 4172  parser = yapx.Ar
+00001aa0: 6775 6d65 6e74 5061 7273 6572 2829 0a20  gumentParser(). 
+00001ab0: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
+00001ac0: 6172 7365 722e 6164 645f 6172 6775 6d65  arser.add_argume
+00001ad0: 6e74 7328 4164 644e 756d 7329 0a20 2020  nts(AddNums).   
+00001ae0: 2020 2020 2020 2020 203e 3e3e 2070 6172           >>> par
+00001af0: 7365 722e 7365 745f 6465 6661 756c 7473  ser.set_defaults
+00001b00: 285f 636f 6d6d 616e 645f 6675 6e63 3d6c  (_command_func=l
+00001b10: 616d 6264 6120 782c 2079 3a20 782b 7929  ambda x, y: x+y)
+00001b20: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00001b30: 2070 6172 7365 6420 3d20 7061 7273 6572   parsed = parser
+00001b40: 2e70 6172 7365 5f61 7267 7328 5b27 2d78  .parse_args(['-x
+00001b50: 272c 2027 3127 2c20 272d 7927 2c20 2732  ', '1', '-y', '2
+00001b60: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
+00001b70: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00001b80: 3e3e 3e20 2870 6172 7365 642e 782c 2070  >>> (parsed.x, p
+00001b90: 6172 7365 642e 7929 0a20 2020 2020 2020  arsed.y).       
+00001ba0: 2020 2020 2028 312c 2032 290a 2020 2020       (1, 2).    
+00001bb0: 2020 2020 2020 2020 3e3e 3e20 7061 7273          >>> pars
+00001bc0: 6564 2e5f 636f 6d6d 616e 645f 6675 6e63  ed._command_func
+00001bd0: 5f61 7267 735f 6d6f 6465 6c28 783d 7061  _args_model(x=pa
+00001be0: 7273 6564 2e78 2c20 793d 7061 7273 6564  rsed.x, y=parsed
+00001bf0: 2e79 290a 2020 2020 2020 2020 2020 2020  .y).            
+00001c00: 4164 644e 756d 7328 783d 312c 2079 3d32  AddNums(x=1, y=2
+00001c10: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00001c20: 3e20 7061 7273 6564 2e5f 636f 6d6d 616e  > parsed._comman
+00001c30: 645f 6675 6e63 2878 3d70 6172 7365 642e  d_func(x=parsed.
+00001c40: 782c 2079 3d70 6172 7365 642e 7929 0a20  x, y=parsed.y). 
+00001c50: 2020 2020 2020 2020 2020 2033 0a0a 2020             3..  
+00001c60: 2020 2020 2020 2020 2020 3e3e 3e20 696d            >>> im
+00001c70: 706f 7274 2079 6170 780a 2020 2020 2020  port yapx.      
+00001c80: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001c90: 2020 2020 2020 3e3e 3e20 6465 6620 6164        >>> def ad
+00001ca0: 645f 6e75 6d73 2878 3a20 696e 742c 2079  d_nums(x: int, y
+00001cb0: 3a20 696e 7429 3a0a 2020 2020 2020 2020  : int):.        
+00001cc0: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
+00001cd0: 726e 2078 202b 2079 0a20 2020 2020 2020  rn x + y.       
+00001ce0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00001cf0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
+00001d00: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
+00001d10: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
+00001d20: 2020 2020 3e3e 3e20 7061 7273 6572 2e61      >>> parser.a
+00001d30: 6464 5f61 7267 756d 656e 7473 2861 6464  dd_arguments(add
+00001d40: 5f6e 756d 7329 0a20 2020 2020 2020 2020  _nums).         
+00001d50: 2020 203e 3e3e 2070 6172 7365 722e 7365     >>> parser.se
+00001d60: 745f 6465 6661 756c 7473 285f 636f 6d6d  t_defaults(_comm
+00001d70: 616e 645f 6675 6e63 3d61 6464 5f6e 756d  and_func=add_num
+00001d80: 7329 0a20 2020 2020 2020 2020 2020 203e  s).            >
+00001d90: 3e3e 2070 6172 7365 6420 3d20 7061 7273  >> parsed = pars
+00001da0: 6572 2e70 6172 7365 5f61 7267 7328 5b27  er.parse_args(['
+00001db0: 2d78 272c 2027 3127 2c20 272d 7927 2c20  -x', '1', '-y', 
+00001dc0: 2732 275d 290a 2020 2020 2020 2020 2020  '2']).          
+00001dd0: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
+00001de0: 2020 3e3e 3e20 2870 6172 7365 642e 782c    >>> (parsed.x,
+00001df0: 2070 6172 7365 642e 7929 0a20 2020 2020   parsed.y).     
+00001e00: 2020 2020 2020 2028 312c 2032 290a 2020         (1, 2).  
+00001e10: 2020 2020 2020 2020 2020 3e3e 3e20 7061            >>> pa
+00001e20: 7273 6564 2e5f 636f 6d6d 616e 645f 6675  rsed._command_fu
+00001e30: 6e63 5f61 7267 735f 6d6f 6465 6c28 783d  nc_args_model(x=
+00001e40: 7061 7273 6564 2e78 2c20 793d 7061 7273  parsed.x, y=pars
+00001e50: 6564 2e79 290a 2020 2020 2020 2020 2020  ed.y).          
+00001e60: 2020 4461 7461 636c 6173 735f 6164 645f    Dataclass_add_
+00001e70: 6e75 6d73 2878 3d31 2c20 793d 3229 0a20  nums(x=1, y=2). 
+00001e80: 2020 2020 2020 2020 2020 203e 3e3e 2070             >>> p
+00001e90: 6172 7365 642e 5f63 6f6d 6d61 6e64 5f66  arsed._command_f
+00001ea0: 756e 6328 783d 7061 7273 6564 2e78 2c20  unc(x=parsed.x, 
+00001eb0: 793d 7061 7273 6564 2e79 290a 2020 2020  y=parsed.y).    
+00001ec0: 2020 2020 2020 2020 330a 2020 2020 2020          3.      
+00001ed0: 2020 4e29 01da 0e5f 6164 645f 6172 6775    N)..._add_argu
+00001ee0: 6d65 6e74 7329 0272 7800 0000 728f 0000  ments).rx...r...
+00001ef0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+00001f00: da0d 6164 645f 6172 6775 6d65 6e74 73f6  ..add_arguments.
+00001f10: 0000 0073 0200 0000 102f 7a1c 4172 6775  ...s...../z.Argu
+00001f20: 6d65 6e74 5061 7273 6572 2e61 6464 5f61  mentParser.add_a
+00001f30: 7267 756d 656e 7473 da04 6e61 6d65 6303  rguments..namec.
+00001f40: 0000 0000 0000 0000 0000 0009 0000 0005  ................
+00001f50: 0000 004b 0000 0073 9800 0000 7c00 a000  ...K...s....|...
+00001f60: a100 7d04 7c02 730b 7401 7c01 6a02 8301  ..}.|.s.t.|.j...
+00001f70: 7d02 7403 7c04 7404 6a05 8302 7313 4a00  }.t.|.t.j...s.J.
+00001f80: 8201 7c03 a006 6401 6402 a102 7d05 7c05  ..|...d.d...}.|.
+00001f90: 7221 7c05 6403 7c02 1700 3700 7d05 7c00  r!|.d.|...7.}.|.
+00001fa0: 6a07 7c01 6404 8d01 7d06 6402 7d07 7c06  j.|.d...}.d.}.|.
+00001fb0: 7231 7c06 a008 a100 6405 1900 7d07 7c04  r1|.....d...}.|.
+00001fc0: 6a09 7c02 6601 7c05 7c07 6406 9c02 7c03  j.|.f.|.|.d...|.
+00001fd0: a401 8e01 7d08 7c06 7242 7c06 7c08 5f0a  ....}.|.rB|.|._.
+00001fe0: 7c01 724a 7c00 a00b 7c08 7c01 a102 0100  |.rJ|...|.|.....
+00001ff0: 7c08 5300 2907 6159 0800 0043 7265 6174  |.S.).aY...Creat
+00002000: 6520 6120 6e65 7720 7375 6263 6f6d 6d61  e a new subcomma
+00002010: 6e64 2061 6e64 2061 6464 2061 7267 756d  nd and add argum
+00002020: 656e 7473 2066 726f 6d20 7468 6520 6769  ents from the gi
+00002030: 7665 6e20 6675 6e63 7469 6f6e 206f 7220  ven function or 
+00002040: 6461 7461 6672 616d 6520 746f 2069 742e  dataframe to it.
+00002050: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00002060: 2020 2020 2020 2020 2020 2020 6172 6773              args
+00002070: 5f6d 6f64 656c 3a20 6120 6675 6e63 7469  _model: a functi
+00002080: 6f6e 206f 7220 6461 7461 636c 6173 7320  on or dataclass 
+00002090: 6672 6f6d 2077 6869 6368 2074 6f20 6465  from which to de
+000020a0: 7269 7665 2061 7267 756d 656e 7473 2e0a  rive arguments..
+000020b0: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+000020c0: 3a20 6e61 6d65 206f 6620 7468 6520 636f  : name of the co
+000020d0: 6d6d 616e 640a 0a20 2020 2020 2020 2052  mmand..        R
+000020e0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000020f0: 2020 2020 7468 6520 6e65 7720 6172 6770      the new argp
+00002100: 6172 7365 2073 7562 7061 7273 6572 0a0a  arse subparser..
+00002110: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00002120: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
+00002130: 3e20 696d 706f 7274 2079 6170 780a 2020  > import yapx.  
+00002140: 2020 2020 2020 2020 2020 3e3e 3e20 6672            >>> fr
+00002150: 6f6d 2064 6174 6163 6c61 7373 6573 2069  om dataclasses i
+00002160: 6d70 6f72 7420 6461 7461 636c 6173 730a  mport dataclass.
+00002170: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00002180: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00002190: 4064 6174 6163 6c61 7373 0a20 2020 2020  @dataclass.     
+000021a0: 2020 2020 2020 202e 2e2e 2063 6c61 7373         ... class
+000021b0: 2041 6464 4e75 6d73 3a0a 2020 2020 2020   AddNums:.      
+000021c0: 2020 2020 2020 2e2e 2e20 2020 2020 783a        ...     x:
+000021d0: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+000021e0: 202e 2e2e 2020 2020 2079 3a20 696e 740a   ...     y: int.
+000021f0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00002200: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00002210: 7061 7273 6572 203d 2079 6170 782e 4172  parser = yapx.Ar
+00002220: 6775 6d65 6e74 5061 7273 6572 2829 0a20  gumentParser(). 
+00002230: 2020 2020 2020 2020 2020 203e 3e3e 2073             >>> s
+00002240: 7562 7061 7273 6572 5f31 203d 2070 6172  ubparser_1 = par
+00002250: 7365 722e 6164 645f 636f 6d6d 616e 6428  ser.add_command(
+00002260: 4164 644e 756d 732c 206e 616d 653d 2761  AddNums, name='a
+00002270: 6464 2729 0a20 2020 2020 2020 2020 2020  dd').           
+00002280: 203e 3e3e 2073 7562 7061 7273 6572 5f31   >>> subparser_1
+00002290: 2e73 6574 5f64 6566 6175 6c74 7328 5f63  .set_defaults(_c
+000022a0: 6f6d 6d61 6e64 5f66 756e 633d 6c61 6d62  ommand_func=lamb
+000022b0: 6461 2078 2c20 793a 2078 2b79 290a 2020  da x, y: x+y).  
+000022c0: 2020 2020 2020 2020 2020 3e3e 3e20 7375            >>> su
+000022d0: 6270 6172 7365 725f 3220 3d20 7061 7273  bparser_2 = pars
+000022e0: 6572 2e61 6464 5f63 6f6d 6d61 6e64 2841  er.add_command(A
+000022f0: 6464 4e75 6d73 2c20 6e61 6d65 3d27 7375  ddNums, name='su
+00002300: 6274 7261 6374 2729 0a20 2020 2020 2020  btract').       
+00002310: 2020 2020 203e 3e3e 2073 7562 7061 7273       >>> subpars
+00002320: 6572 5f32 2e73 6574 5f64 6566 6175 6c74  er_2.set_default
+00002330: 7328 5f63 6f6d 6d61 6e64 5f66 756e 633d  s(_command_func=
+00002340: 6c61 6d62 6461 2078 2c20 793a 2078 2d79  lambda x, y: x-y
+00002350: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
+00002360: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00002370: 3e20 7061 7273 6564 203d 2070 6172 7365  > parsed = parse
+00002380: 722e 7061 7273 655f 6172 6773 285b 2761  r.parse_args(['a
+00002390: 6464 272c 2027 2d78 272c 2027 3127 2c20  dd', '-x', '1', 
+000023a0: 272d 7927 2c20 2732 275d 290a 2020 2020  '-y', '2']).    
+000023b0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+000023c0: 2020 2020 2020 2020 3e3e 3e20 2870 6172          >>> (par
+000023d0: 7365 642e 782c 2070 6172 7365 642e 7929  sed.x, parsed.y)
+000023e0: 0a20 2020 2020 2020 2020 2020 2028 312c  .            (1,
+000023f0: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
+00002400: 3e3e 3e20 7061 7273 6564 2e5f 636f 6d6d  >>> parsed._comm
+00002410: 616e 645f 6675 6e63 5f61 7267 735f 6d6f  and_func_args_mo
+00002420: 6465 6c28 783d 7061 7273 6564 2e78 2c20  del(x=parsed.x, 
+00002430: 793d 7061 7273 6564 2e79 290a 2020 2020  y=parsed.y).    
+00002440: 2020 2020 2020 2020 4164 644e 756d 7328          AddNums(
+00002450: 783d 312c 2079 3d32 290a 2020 2020 2020  x=1, y=2).      
+00002460: 2020 2020 2020 3e3e 3e20 7061 7273 6564        >>> parsed
+00002470: 2e5f 636f 6d6d 616e 645f 6675 6e63 2878  ._command_func(x
+00002480: 3d70 6172 7365 642e 782c 2079 3d70 6172  =parsed.x, y=par
+00002490: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
+000024a0: 2020 2033 0a0a 2020 2020 2020 2020 2020     3..          
+000024b0: 2020 3e3e 3e20 696d 706f 7274 2079 6170    >>> import yap
+000024c0: 780a 2020 2020 2020 2020 2020 2020 2e2e  x.            ..
+000024d0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+000024e0: 3e20 6465 6620 6164 645f 6e75 6d73 2878  > def add_nums(x
+000024f0: 3a20 696e 742c 2079 3a20 696e 7429 3a0a  : int, y: int):.
+00002500: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00002510: 2020 2020 7265 7475 726e 2078 202b 2079      return x + y
+00002520: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00002530: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00002540: 2064 6566 2073 7562 7472 6163 745f 6e75   def subtract_nu
+00002550: 6d73 2878 3a20 696e 742c 2079 3a20 696e  ms(x: int, y: in
+00002560: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+00002570: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
+00002580: 202d 2079 0a20 2020 2020 2020 2020 2020   - y.           
+00002590: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+000025a0: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
+000025b0: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
+000025c0: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+000025d0: 3e3e 3e20 7375 6270 6172 7365 725f 3120  >>> subparser_1 
+000025e0: 3d20 7061 7273 6572 2e61 6464 5f63 6f6d  = parser.add_com
+000025f0: 6d61 6e64 2861 6464 5f6e 756d 732c 206e  mand(add_nums, n
+00002600: 616d 653d 2761 6464 2729 0a20 2020 2020  ame='add').     
+00002610: 2020 2020 2020 203e 3e3e 2073 7562 7061         >>> subpa
+00002620: 7273 6572 5f31 2e73 6574 5f64 6566 6175  rser_1.set_defau
+00002630: 6c74 7328 5f63 6f6d 6d61 6e64 5f66 756e  lts(_command_fun
+00002640: 633d 6164 645f 6e75 6d73 290a 2020 2020  c=add_nums).    
+00002650: 2020 2020 2020 2020 3e3e 3e20 7375 6270          >>> subp
+00002660: 6172 7365 725f 3220 3d20 7061 7273 6572  arser_2 = parser
+00002670: 2e61 6464 5f63 6f6d 6d61 6e64 2873 7562  .add_command(sub
+00002680: 7472 6163 745f 6e75 6d73 2c20 6e61 6d65  tract_nums, name
+00002690: 3d27 7375 6274 7261 6374 2729 0a20 2020  ='subtract').   
+000026a0: 2020 2020 2020 2020 203e 3e3e 2073 7562           >>> sub
+000026b0: 7061 7273 6572 5f32 2e73 6574 5f64 6566  parser_2.set_def
+000026c0: 6175 6c74 7328 5f63 6f6d 6d61 6e64 5f66  aults(_command_f
+000026d0: 756e 633d 7375 6274 7261 6374 5f6e 756d  unc=subtract_num
+000026e0: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
+000026f0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
+00002700: 3e3e 2070 6172 7365 6420 3d20 7061 7273  >> parsed = pars
+00002710: 6572 2e70 6172 7365 5f61 7267 7328 5b27  er.parse_args(['
+00002720: 7375 6274 7261 6374 272c 2027 2d78 272c  subtract', '-x',
+00002730: 2027 3127 2c20 272d 7927 2c20 2732 275d   '1', '-y', '2']
+00002740: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
+00002750: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00002760: 3e20 2870 6172 7365 642e 782c 2070 6172  > (parsed.x, par
+00002770: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
+00002780: 2020 2028 312c 2032 290a 2020 2020 2020     (1, 2).      
+00002790: 2020 2020 2020 3e3e 3e20 7061 7273 6564        >>> parsed
+000027a0: 2e5f 636f 6d6d 616e 645f 6675 6e63 5f61  ._command_func_a
+000027b0: 7267 735f 6d6f 6465 6c28 783d 7061 7273  rgs_model(x=pars
+000027c0: 6564 2e78 2c20 793d 7061 7273 6564 2e79  ed.x, y=parsed.y
+000027d0: 290a 2020 2020 2020 2020 2020 2020 4461  ).            Da
+000027e0: 7461 636c 6173 735f 7375 6274 7261 6374  taclass_subtract
+000027f0: 5f6e 756d 7328 783d 312c 2079 3d32 290a  _nums(x=1, y=2).
+00002800: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00002810: 7061 7273 6564 2e5f 636f 6d6d 616e 645f  parsed._command_
+00002820: 6675 6e63 2878 3d70 6172 7365 642e 782c  func(x=parsed.x,
+00002830: 2079 3d70 6172 7365 642e 7929 0a20 2020   y=parsed.y).   
+00002840: 2020 2020 2020 2020 202d 310a 2020 2020           -1.    
+00002850: 2020 2020 7247 0000 004e fa01 20a9 0172      rG...N.. ..r
+00002860: 8f00 0000 7201 0000 0029 0272 4700 0000  ....r....).rG...
+00002870: 725a 0000 0029 0c72 7700 0000 7224 0000  rZ...).rw...r$..
+00002880: 00da 085f 5f6e 616d 655f 5f72 6d00 0000  ...__name__rm...
+00002890: 7274 0000 00da 115f 5375 6250 6172 7365  rt....._SubParse
+000028a0: 7273 4163 7469 6f6e da03 706f 70da 1f5f  rsAction..pop.._
+000028b0: 6765 745f 6465 7363 7269 7074 696f 6e5f  get_description_
+000028c0: 6672 6f6d 5f64 6f63 7374 7269 6e67 da0a  from_docstring..
+000028d0: 7370 6c69 746c 696e 6573 da0a 6164 645f  splitlines..add_
+000028e0: 7061 7273 6572 7249 0000 0072 9000 0000  parserrI...r....
+000028f0: 2909 7278 0000 0072 8f00 0000 7292 0000  ).rx...r....r...
+00002900: 0072 5100 0000 5a0a 7375 6270 6172 7365  .rQ...Z.subparse
+00002910: 7273 7247 0000 005a 0f64 6573 6372 6970  rsrG...Z.descrip
+00002920: 7469 6f6e 5f74 7874 5a08 6865 6c70 5f74  tion_txtZ.help_t
+00002930: 7874 7266 0000 0072 5300 0000 7253 0000  xtrf...rS...rS..
+00002940: 0072 5700 0000 da0b 6164 645f 636f 6d6d  .rW.....add_comm
+00002950: 616e 6427 0100 0073 3400 0000 083e 0402  and'...s4....>..
+00002960: 0a01 1003 0c01 0401 0c01 0404 0201 06ff  ................
+00002970: 0403 0401 0c01 0402 0201 02ff 0202 0201  ................
+00002980: 04fd 0204 06fc 0406 0601 0402 0c01 0402  ................
+00002990: 7a1a 4172 6775 6d65 6e74 5061 7273 6572  z.ArgumentParser
+000029a0: 2e61 6464 5f63 6f6d 6d61 6e64 da04 6675  .add_command..fu
+000029b0: 6e63 6303 0000 0000 0000 0000 0000 0005  ncc.............
+000029c0: 0000 0005 0000 004b 0000 0073 4200 0000  .......K...sB...
+000029d0: 7400 7c02 7205 7c02 6e02 7c01 6a01 8301  t.|.r.|.n.|.j...
+000029e0: 7d02 7c00 6a02 7c01 6601 6401 7c02 6901  }.|.j.|.f.d.|.i.
+000029f0: 7c03 a401 8e01 7d04 7c04 6a03 6402 6900  |.....}.|.j.d.i.
+00002a00: 7c00 6a04 7c01 6901 a401 8e01 0100 6400  |.j.|.i.......d.
+00002a10: 5300 2903 4e72 9200 0000 7253 0000 0029  S.).Nr....rS...)
+00002a20: 0572 2400 0000 7295 0000 0072 9b00 0000  .r$...r....r....
+00002a30: da0c 7365 745f 6465 6661 756c 7473 7245  ..set_defaultsrE
+00002a40: 0000 0029 0572 7800 0000 729c 0000 0072  ...).rx...r....r
+00002a50: 9200 0000 7251 0000 0072 6600 0000 7253  ....rQ...rf...rS
+00002a60: 0000 0072 5300 0000 7257 0000 00da 115f  ...rS...rW....._
+00002a70: 7265 6769 7374 6572 5f63 6f6d 6d61 6e64  register_command
+00002a80: 8701 0000 7312 0000 0012 0604 0102 0104  ....s...........
+00002a90: ff02 0202 fe02 0306 fd1a 057a 2041 7267  ...........z Arg
+00002aa0: 756d 656e 7450 6172 7365 722e 5f72 6567  umentParser._reg
+00002ab0: 6973 7465 725f 636f 6d6d 616e 64da 0464  ister_command..d
+00002ac0: 636c 73da 0461 7474 7263 0200 0000 0000  cls..attrc......
+00002ad0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+00002ae0: 0000 730a 0000 007c 017c 006a 0076 0153  ..s....|.|.j.v.S
+00002af0: 0072 5c00 0000 a901 da0f 5f5f 616e 6e6f  .r\.......__anno
+00002b00: 7461 7469 6f6e 735f 5fa9 0272 9f00 0000  tations__..r....
+00002b10: 72a0 0000 0072 5300 0000 7253 0000 0072  r....rS...rS...r
+00002b20: 5700 0000 da17 5f69 735f 6174 7472 6962  W....._is_attrib
+00002b30: 7574 655f 696e 6865 7269 7465 6495 0100  ute_inherited...
+00002b40: 0073 0200 0000 0a02 7a26 4172 6775 6d65  .s......z&Argume
+00002b50: 6e74 5061 7273 6572 2e5f 6973 5f61 7474  ntParser._is_att
+00002b60: 7269 6275 7465 5f69 6e68 6572 6974 6564  ribute_inherited
+00002b70: 7266 0000 0063 0300 0000 0000 0000 0000  rf...c..........
+00002b80: 0000 1900 0000 0900 0000 0300 0000 73f2  ..............s.
+00002b90: 0600 0074 007c 0283 0172 077c 0289 016e  ...t.|...r.|...n
+00002ba0: 0474 017c 0283 0189 017c 01a0 0288 006a  .t.|.....|.....j
+00002bb0: 03a1 0172 1864 017d 037c 01a0 047c 03a1  ...r.d.}.|...|..
+00002bc0: 0101 007c 016a 0564 2269 0088 006a 0388  ...|.j.d"i...j..
+00002bd0: 0169 01a4 018e 0101 0069 007d 0474 0674  .i.......i.}.t.t
+00002be0: 0787 0087 0166 0264 0264 0384 0874 0888  .....f.d.d...t..
+00002bf0: 0183 0183 0283 017d 0564 0464 0584 007c  .......}.d.d...|
+00002c00: 0544 0083 017d 0667 007d 077c 0644 0090  .D...}.g.}.|.D..
+00002c10: 035d 375c 027d 087d 097c 086a 097d 0a74  .]7\.}.}.|.j.}.t
+00002c20: 0a7c 0a74 0b83 0272 4f74 0c7c 0a83 017d  .|.t...rOt.|...}
+00002c30: 0a74 0a7c 0a74 0b83 0272 564a 0082 0174  .t.|.t...rVJ...t
+00002c40: 0d6a 0e64 066b 0572 6074 0a7c 0a74 0f83  .j.d.k.r`t.|.t..
+00002c50: 0273 6788 00a0 107c 0aa1 0174 1175 0072  .sg....|...t.u.r
+00002c60: 6e88 006a 127c 0a64 0764 088d 027d 0a74  n..j.|.d.d...}.t
+00002c70: 0a7c 0a74 1383 0272 a988 00a0 147c 0aa1  .|.t...r.....|..
+00002c80: 0144 005d 137d 0b74 157c 0b74 1683 0272  .D.].}.t.|.t...r
+00002c90: 8b74 177c 0b6a 1876 0072 8b7c 0b6a 1874  .t.|.j.v.r.|.j.t
+00002ca0: 1719 007d 0901 006e 0171 7888 00a0 107c  ...}...n.qx....|
+00002cb0: 0aa1 017d 0a74 0d6a 0e64 066b 0572 9b74  ...}.t.j.d.k.r.t
+00002cc0: 0a7c 0a74 0f83 0273 a288 00a0 107c 0aa1  .|.t...s.....|..
+00002cd0: 0174 1175 0072 a988 006a 127c 0a64 0764  .t.u.r...j.|.d.d
+00002ce0: 088d 027d 0a74 0a7c 0a74 0983 0272 b17c  ...}.t.|.t...r.|
+00002cf0: 0a6a 196e 0a74 0b7c 0a83 016a 1a64 0964  .j.n.t.|...j.d.d
+00002d00: 0a64 0b8d 0264 0c19 007d 0c7c 09a0 1b7c  .d...d...}.|...|
+00002d10: 086a 1ca1 0101 007c 096a 1d72 df7c 086a  .j.....|.j.r.|.j
+00002d20: 1e74 1f75 0172 d27c 086a 1e7c 095f 1e64  .t.u.r.|.j.|._.d
+00002d30: 0d7c 095f 1d6e 0d7c 086a 2074 1f75 0172  .|._.n.|.j t.u.r
+00002d40: df7c 08a0 20a1 007c 095f 1e64 0d7c 095f  .|.. ..|._.d.|._
+00002d50: 1d88 00a0 107c 0aa1 017d 0d7c 0d90 0172  .....|...}.|...r
+00002d60: 6f7c 0d90 0172 037c 0d74 2175 0090 0172  o|...r.|.t!u...r
+00002d70: 0374 0688 00a0 227c 0aa1 0183 017c 095f  .t...."|.....|._
+00002d80: 237c 096a 2390 0172 0274 097c 096a 2364  #|.j#..r.t.|.j#d
+00002d90: 0e19 0083 017d 0a6e 7774 247c 0d74 256a  .....}.nwt$|.t%j
+00002da0: 266a 2783 0290 0172 1a88 006a 127c 0a64  &j'....r...j.|.d
+00002db0: 0764 0f8d 027d 0a7c 096a 2890 0173 1974  .d...}.|.j(..s.t
+00002dc0: 297c 095f 286e 3574 247c 0d74 256a 266a  )|._(n5t$|.t%j&j
+00002dd0: 2a83 0290 0173 277c 0d74 2b75 0090 0172  *....s'|.t+u...r
+00002de0: 4888 006a 127c 0a64 0764 0f8d 027d 0a7c  H..j.|.d.d...}.|
+00002df0: 096a 2890 0173 477c 0d74 2b75 0090 0172  .j(..sG|.t+u...r
+00002e00: 3b74 2c7c 095f 286e 147c 0d74 2d75 0090  ;t,|._(n.|.t-u..
+00002e10: 0172 4474 2e7c 095f 286e 0b74 2f7c 095f  .rDt.|._(n.t/|._
+00002e20: 286e 0774 3090 0173 4f74 317c 0a83 0101  (n.t0..sOt1|....
+00002e30: 0074 247c 0a74 3283 0290 0172 5d64 1064  .t$|.t2....r]d.d
+00002e40: 0584 007c 0a44 0083 017c 095f 2374 157c  ...|.D...|._#t.|
+00002e50: 0188 0083 0290 0172 6c74 3374 347c 0a83  .......rlt3t4|..
+00002e60: 027c 016a 357c 096a 363c 0074 0b7d 0a6e  .|.j5|.j6<.t.}.n
+00002e70: 0b74 247c 0a74 3283 0290 0172 7a74 067c  .t$|.t2....rzt.|
+00002e80: 0a83 017c 095f 237c 0a7c 095f 097c 09a0  ...|._#|.|._.|..
+00002e90: 37a1 007d 0e7c 0e64 113d 007c 0ea0 3864  7..}.|.d.=.|..8d
+00002ea0: 12a1 017d 0f7c 0f90 0173 8e67 006e 0664  ...}.|...s.g.n.d
+00002eb0: 1364 0584 007c 0f44 0083 017d 107c 0e64  .d...|.D...}.|.d
+00002ec0: 1419 0090 0173 b17c 0ea0 3964 15a1 0190  .....s.|..9d....
+00002ed0: 0173 b17c 1090 0173 ad64 167c 0e64 1719  .s.|...s.d.|.d..
+00002ee0: 00a0 3aa1 009b 0064 189d 036e 0164 197c  ..:....d...n.d.|
+00002ef0: 0e64 143c 007c 0e64 1a19 007d 117c 1090  .d.<.|.d...}.|..
+00002f00: 0173 d27c 0e64 1a3d 007c 1190 0173 ca7c  .s.|.d.=.|...s.|
+00002f10: 0ea0 3964 1ba1 0164 0075 0090 0172 ca64  ..9d...d.u...r.d
+00002f20: 1c7c 0e64 1b3c 0074 3374 347c 0a83 027c  .|.d.<.t3t4|...|
+00002f30: 0e64 1d3c 006e 4c7c 096a 0974 3b75 0090  .d.<.nL|.j.t;u..
+00002f40: 0172 fd74 157c 0188 0083 0290 0172 e774  .r.t.|.......r.t
+00002f50: 3374 347c 0a83 027c 016a 357c 096a 363c  3t4|...|.j5|.j6<
+00002f60: 0064 1e44 005d 097d 127c 0ea0 387c 1264  .d.D.].}.|..8|.d
+00002f70: 00a1 0201 0090 0171 e97c 0e64 1f19 0090  .......q.|.d....
+00002f80: 0173 fc74 3c7c 0e64 1f3c 006e 217c 096a  .s.t<|.d.<.n!|.j
+00002f90: 3d64 0e6b 0390 0272 0b74 3374 347c 0a83  =d.k...r.t3t4|..
+00002fa0: 027c 0e64 1d3c 006e 137c 0a74 3e75 0090  .|.d.<.n.|.t>u..
+00002fb0: 0272 1574 3f7c 0e64 1f3c 006e 097c 0a74  .r.t?|.d.<.n.|.t
+00002fc0: 0b75 0090 0272 1e74 407c 0e64 1f3c 007c  .u...r.t@|.d.<.|
+00002fd0: 086a 1e74 1f75 0190 0273 327c 086a 2074  .j.t.u...s2|.j t
+00002fe0: 1f75 0190 0273 327c 0ea0 3964 20a1 0164  .u...s2|..9d ..d
+00002ff0: 0075 0190 0272 c97c 0ea0 3964 1fa1 0190  .u...r.|..9d....
+00003000: 0272 6574 247c 0e64 1f19 0074 416a 4274  .ret$|.d...tAjBt
+00003010: 3c66 0283 0290 0272 6574 0964 2164 2269  <f.....ret.d!d"i
+00003020: 0083 0383 007d 137c 0e64 1f19 007c 107c  .....}.|.d...|.|
+00003030: 0e64 1719 0064 238d 027c 017c 137c 0e64  .d...d#..|.|.|.d
+00003040: 2019 0064 248d 0301 0074 437c 137c 0e64   ..d$....tC|.|.d
+00003050: 1719 0083 027c 0e64 203c 006e 0f64 1d7c  .....|.d <.n.d.|
+00003060: 0e76 0090 0272 747c 0e64 1d19 007c 0e64  .v...rt|.d...|.d
+00003070: 2019 0083 017c 0e64 203c 007c 0ea0 3964   ....|.d <.|..9d
+00003080: 15a1 0190 0272 c97c 0e64 2019 007d 1474  .....r.|.d ..}.t
+00003090: 0a7c 1474 0b83 0290 0273 8c74 0a7c 1474  .|.t.....s.t.|.t
+000030a0: 256a 266a 2a83 0290 0273 8f7c 1467 017d  %j&j*....s.|.g.}
+000030b0: 147c 1444 005d 377d 0b7c 0b7c 0e64 1519  .|.D.]7}.|.|.d..
+000030c0: 0076 0190 0272 c774 0a7c 0b74 3283 0290  .v...r.t.|.t2...
+000030d0: 0272 a87c 0b6a 1c7c 0e64 1519 0076 0190  .r.|.j.|.d...v..
+000030e0: 0272 c77c 0ea0 3964 1aa1 0190 0273 b37c  .r.|..9d.....s.|
+000030f0: 0b64 0075 0090 0273 c764 257c 0b9b 0064  .d.u...s.d%|...d
+00003100: 267c 0e64 1719 009b 0064 277c 0e64 1519  &|.d.....d'|.d..
+00003110: 009b 009d 067d 037c 01a0 047c 03a1 0101  .....}.|...|....
+00003120: 0090 0271 9164 287c 0c9b 009d 0267 017d  ...q.d(|.....g.}
+00003130: 157c 1190 0273 e674 157c 0ea0 3964 20a1  .|...s.t.|..9d .
+00003140: 0174 0b83 0290 0272 e17c 15a0 4464 29a1  .t.....r.|..Dd).
+00003150: 0101 006e 057c 15a0 4464 2aa1 0101 007c  ...n.|..Dd*....|
+00003160: 0ea0 3864 2b64 0da1 0290 0272 f27c 15a0  ..8d+d.....r.|..
+00003170: 4464 2ca1 0101 007c 096a 4590 0272 ff7c  Dd,....|.jE..r.|
+00003180: 15a0 4464 2d7c 096a 459b 009d 02a1 0101  ..Dd-|.jE.......
+00003190: 0064 2e64 2fa0 467c 15a1 019b 009d 027d  .d.d/.F|.......}
+000031a0: 167c 0ea0 3964 30a1 0190 0372 187c 0e64  .|..9d0....r.|.d
+000031b0: 3005 0019 0064 317c 1617 0037 0003 003c  0....d1|...7...<
+000031c0: 006e 047c 167c 0e64 303c 007c 0ea0 3864  .n.|.|.d0<.|..8d
+000031d0: 3264 00a1 027d 177c 1790 0373 2c7c 1190  2d...}.|...s,|..
+000031e0: 0372 2a64 336e 0164 347d 177c 04a0 397c  .r*d3n.d4}.|..9|
+000031f0: 1764 00a1 027d 187c 1890 0373 3e7c 01a0  .d...}.|...s>|..
+00003200: 477c 17a1 017d 187c 187c 047c 173c 007c  G|...}.|.|.|.<.|
+00003210: 096a 4890 0372 697c 1190 0372 5064 357c  .jH..ri|...rPd5|
+00003220: 096a 369b 009d 027d 037c 01a0 047c 03a1  .j6....}.|...|..
+00003230: 0101 007c 016a 497c 016a 4aa0 3988 006a  ...|.jI|.jJ.9..j
+00003240: 4ba1 0119 007c 1719 00a0 447c 096a 367c  K....|....D|.j6|
+00003250: 1090 0372 657c 1064 0c19 006e 0164 0066  ...re|.d...n.d.f
+00003260: 02a1 0101 007c 186a 4c7c 1069 007c 0ea4  .....|.jL|.i.|..
+00003270: 018e 0101 007c 07a0 447c 09a1 0101 0071  .....|..D|.....q
+00003280: 3e7c 0753 0029 364e 7a3e 5468 6973 2070  >|.S.)6Nz>This p
+00003290: 6172 7365 7220 616c 7265 6164 7920 636f  arser already co
+000032a0: 6e74 6169 6e73 2061 7267 756d 656e 7473  ntains arguments
+000032b0: 2066 726f 6d20 616e 6f74 6865 7220 6461   from another da
+000032c0: 7461 636c 6173 732e 6301 0000 0000 0000  taclass.c.......
+000032d0: 0000 0000 0001 0000 0004 0000 0013 0000  ................
+000032e0: 0073 1200 0000 8800 6a00 8801 7c00 6a01  .s......j...|.j.
+000032f0: 6401 8d02 0c00 5300 2902 4e72 a300 0000  d.....S.).Nr....
+00003300: 2902 72a4 0000 0072 9200 0000 2901 da01  ).r....r....)...
+00003310: 66a9 02da 0363 6c73 5a05 6d6f 6465 6c72  f....clsZ.modelr
+00003320: 5300 0000 7257 0000 0072 5e00 0000 b201  S...rW...r^.....
+00003330: 0000 f302 0000 0012 007a 2f41 7267 756d  .........z/Argum
+00003340: 656e 7450 6172 7365 722e 5f61 6464 5f61  entParser._add_a
+00003350: 7267 756d 656e 7473 2e3c 6c6f 6361 6c73  rguments.<locals
+00003360: 3e2e 3c6c 616d 6264 613e 6301 0000 0000  >.<lambda>c.....
+00003370: 0000 0000 0000 0002 0000 0007 0000 0053  ...............S
+00003380: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
+00003390: 7c01 7c01 6a00 a001 7402 7403 8300 a102  |.|.j...t.t.....
+000033a0: 6602 9102 7102 5300 7253 0000 0029 04da  f...q.S.rS...)..
+000033b0: 086d 6574 6164 6174 61da 0367 6574 7221  .metadata..getr!
+000033c0: 0000 0072 2200 0000 7254 0000 0072 5300  ...r"...rT...rS.
+000033d0: 0000 7253 0000 0072 5700 0000 7258 0000  ..rS...rW...rX..
+000033e0: 00b7 0100 0073 0800 0000 0600 0202 12ff  .....s..........
+000033f0: 06ff 7a31 4172 6775 6d65 6e74 5061 7273  ..z1ArgumentPars
+00003400: 6572 2e5f 6164 645f 6172 6775 6d65 6e74  er._add_argument
+00003410: 732e 3c6c 6f63 616c 733e 2e3c 6c69 7374  s.<locals>.<list
+00003420: 636f 6d70 3e72 3d00 0000 5429 01da 0d69  comp>r=...T)...i
+00003430: 735f 756e 696f 6e5f 7479 7065 da01 2e72  s_union_type...r
+00003440: 1700 0000 a901 da08 6d61 7873 706c 6974  ........maxsplit
+00003450: e9ff ffff ff46 7201 0000 0029 01da 1061  .....Fr....)...a
+00003460: 7373 6572 745f 7072 696d 6974 6976 6563  ssert_primitivec
+00003470: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00003480: 0300 0000 5300 0000 7312 0000 0067 007c  ....S...s....g.|
+00003490: 005d 057d 017c 016a 0091 0271 0253 0072  .].}.|.j...q.S.r
+000034a0: 5300 0000 a901 7292 0000 0072 5400 0000  S.....r....rT...
+000034b0: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+000034c0: 5800 0000 1302 0000 72a8 0000 00da 0370  X.......r......p
+000034d0: 6f73 7267 0000 0063 0100 0000 0000 0000  osrg...c........
+000034e0: 0000 0000 0200 0000 0500 0000 5300 0000  ............S...
+000034f0: 731a 0000 0067 007c 005d 097d 017c 01a0  s....g.|.].}.|..
+00003500: 0064 00a1 0172 027c 0191 0271 0253 0029  .d...r.|...q.S.)
+00003510: 0172 6500 0000 725f 0000 0072 5400 0000  .re...r_...rT...
+00003520: 7253 0000 0072 5300 0000 7257 0000 0072  rS...rS...rW...r
+00003530: 5800 0000 2d02 0000 7302 0000 001a 00da  X...-...s.......
+00003540: 076d 6574 6176 6172 7264 0000 00fa 013c  .metavarrd.....<
+00003550: da04 6465 7374 fa01 3e7a 073c 7661 6c75  ..dest..>z.<valu
+00003560: 653e da08 7265 7175 6972 6564 da05 6e61  e>..required..na
+00003570: 7267 73fa 013f da04 7479 7065 2905 72ba  rgs..?..type).r.
+00003580: 0000 0072 b800 0000 da05 636f 6e73 7472  ...r......constr
+00003590: 6400 0000 72b3 0000 0072 5900 0000 7263  d...r....rY...rc
+000035a0: 0000 00da 0072 5300 0000 2902 7267 0000  .....rS...).rg..
+000035b0: 0072 b500 0000 2903 7266 0000 00da 096e  .r....).rf.....n
+000035c0: 616d 6573 7061 6365 da06 7661 6c75 6573  amespace..values
+000035d0: 7a0f 496e 7661 6c69 6420 7661 6c75 6520  z.Invalid value 
+000035e0: 277a 1027 2066 6f72 2061 7267 756d 656e  'z.' for argumen
+000035f0: 7420 277a 1327 3b20 6d75 7374 2062 6520  t 'z.'; must be 
+00003600: 6f6e 6520 6f66 3a20 7a06 5479 7065 3a20  one of: z.Type: 
+00003610: 7a16 4465 6661 756c 743a 2022 2528 6465  z.Default: "%(de
+00003620: 6661 756c 7429 7322 7a14 4465 6661 756c  fault)s"z.Defaul
+00003630: 743a 2025 2864 6566 6175 6c74 2973 da09  t: %(default)s..
+00003640: 6578 636c 7573 6976 657a 044d 2e58 2e7a  exclusivez.M.X.z
+00003650: 0545 6e76 3a20 7a02 3e20 fa02 2c20 725a  .Env: z.> .., rZ
+00003660: 0000 0072 7d00 0000 da05 6772 6f75 707a  ...r}.....groupz
+00003670: 1372 6571 7569 7265 6420 7061 7261 6d65  .required parame
+00003680: 7465 7273 7a13 6f70 7469 6f6e 616c 2070  tersz.optional p
+00003690: 6172 616d 6574 6572 737a 3341 206d 7574  arametersz3A mut
+000036a0: 7561 6c6c 792d 6578 636c 7573 6976 6520  ually-exclusive 
+000036b0: 7061 7261 6d65 7465 7220 6361 6e6e 6f74  parameter cannot
+000036c0: 2062 6520 7265 7175 6972 6564 3a20 294d   be required: )M
+000036d0: 7234 0000 0072 2500 0000 da0b 6765 745f  r4...r%.....get_
+000036e0: 6465 6661 756c 7472 4600 0000 7282 0000  defaultrF...r...
+000036f0: 0072 9d00 0000 725d 0000 00da 0666 696c  .r....r].....fil
+00003700: 7465 7272 0600 0000 72ba 0000 0072 3800  terr....r....r8.
+00003710: 0000 726e 0000 0072 2300 0000 727f 0000  ..rn...r#...r...
+00003720: 00da 0c76 6572 7369 6f6e 5f69 6e66 6f72  ...version_infor
+00003730: 3f00 0000 da10 5f67 6574 5f74 7970 655f  ?....._get_type_
+00003740: 6f72 6967 696e 7215 0000 00da 1c5f 6578  originr......_ex
+00003750: 7472 6163 745f 7479 7065 5f66 726f 6d5f  tract_type_from_
+00003760: 636f 6e74 6169 6e65 7272 3c00 0000 da12  containerr<.....
+00003770: 5f67 6574 5f74 7970 655f 6d65 7461 6461  _get_type_metada
+00003780: 7461 726d 0000 0072 0500 0000 7221 0000  tarm...r....r!..
+00003790: 0072 a900 0000 7295 0000 00da 0672 7370  .r....r......rsp
+000037a0: 6c69 74da 0873 6574 5f64 6573 7472 9200  lit..set_destr..
+000037b0: 0000 72b7 0000 0072 6300 0000 7204 0000  ..r....rc...r...
+000037c0: 00da 0f64 6566 6175 6c74 5f66 6163 746f  ...default_facto
+000037d0: 7279 722a 0000 00da 0e5f 6765 745f 7479  ryr*....._get_ty
+000037e0: 7065 5f61 7267 7372 6400 0000 7239 0000  pe_argsrd...r9..
+000037f0: 00da 0b63 6f6c 6c65 6374 696f 6e73 da03  ...collections..
+00003800: 6162 63da 074d 6170 7069 6e67 7259 0000  abc..MappingrY..
+00003810: 0072 1d00 0000 da08 4974 6572 6162 6c65  .r......Iterable
+00003820: da03 7365 7472 1f00 0000 da05 7475 706c  ..setr......tupl
+00003830: 6572 2000 0000 721e 0000 0072 3500 0000  er ...r....r5...
+00003840: 7227 0000 0072 0700 0000 7208 0000 0072  r'...r....r....r
+00003850: 3100 0000 7272 0000 0072 b500 0000 da06  1...rr...r......
+00003860: 6173 6469 6374 7297 0000 0072 aa00 0000  asdictr....r....
+00003870: da05 7570 7065 72da 0462 6f6f 6c72 1800  ..upper..boolr..
+00003880: 0000 72b8 0000 00da 0369 6e74 7219 0000  ..r......intr...
+00003890: 0072 1a00 0000 7274 0000 00da 0641 6374  .r....rt.....Act
+000038a0: 696f 6eda 0767 6574 6174 7472 da06 6170  ion..getattr..ap
+000038b0: 7065 6e64 da08 5f65 6e76 5f76 6172 da04  pend.._env_var..
+000038c0: 6a6f 696e da12 6164 645f 6172 6775 6d65  join..add_argume
+000038d0: 6e74 5f67 726f 7570 72bf 0000 0072 7100  nt_groupr....rq.
+000038e0: 0000 da09 5f64 6566 6175 6c74 7372 4500  ...._defaultsrE.
+000038f0: 0000 726f 0000 0029 1972 a700 0000 7266  ..ro...).r....rf
+00003900: 0000 0072 8f00 0000 da03 6572 725a 1170  ...r......errZ.p
+00003910: 6172 7365 725f 6172 675f 6772 6f75 7073  arser_arg_groups
+00003920: 5a0c 6e6f 7665 6c5f 6669 656c 6473 5a10  Z.novel_fieldsZ.
+00003930: 6e6f 7665 6c5f 6669 656c 645f 6172 6773  novel_field_args
+00003940: 5a0a 6164 6465 645f 6172 6773 5a03 666c  Z.added_argsZ.fl
+00003950: 645a 1161 7267 7061 7273 655f 6172 6775  dZ.argparse_argu
+00003960: 6d65 6e74 da08 666c 645f 7479 7065 7256  ment..fld_typerV
+00003970: 0000 005a 0968 656c 705f 7479 7065 5a0f  ...Z.help_typeZ.
+00003980: 666c 645f 7479 7065 5f6f 7269 6769 6e72  fld_type_originr
+00003990: 5100 0000 7267 0000 0072 5000 0000 72b7  Q...rg...rP...r.
+000039a0: 0000 00da 016b 5a0f 6475 6d6d 795f 6e61  .....kZ.dummy_na
+000039b0: 6d65 7370 6163 65da 0164 5a0e 6865 6c70  mespace..dZ.help
+000039c0: 5f6d 7367 5f70 6172 7473 5a08 6865 6c70  _msg_partsZ.help
+000039d0: 5f6d 7367 72c1 0000 005a 0961 7267 5f67  _msgr....Z.arg_g
+000039e0: 726f 7570 7253 0000 0072 a600 0000 7257  rouprS...r....rW
+000039f0: 0000 0072 9000 0000 9901 0000 739c 0100  ...r........s...
+00003a00: 0008 0a06 0108 020c 0204 010a 0116 0204  ................
+00003a10: 0202 0202 010c 0106 0102 fe04 ff06 0702  ................
+00003a20: 0206 fe04 050e 0206 010a 0408 010e 0114  ................
+00003a30: 030e 0104 0102 0102 0106 fe0a 050e 0114  ................
+00003a40: 010a 0104 0102 800a 0214 030e 0104 0102  ................
+00003a50: 0102 0106 fe08 0708 ff14 0202 fd0c 0606  ................
+00003a60: 020a 0108 0108 010a 010a 0106 010a 0206  ................
+00003a70: 0110 0110 0108 010e 0102 8010 0304 0102  ................
+00003a80: 0102 0106 fe08 0406 0102 800c 0304 ff0a  ................
+00003a90: 0204 0202 0102 0106 fe08 040a 0108 010a  ................
+00003aa0: 0108 0106 0202 8006 0208 010c 0210 010c  ................
+00003ab0: 0202 0302 0102 010c fe06 070c 020a 0106  ................
+00003ac0: 0208 0206 010a 0202 0308 ff0c 0202 fd16  ................
+00003ad0: 061c 0206 ff08 0406 0206 0216 0108 0110  ................
+00003ae0: 010c 010c 0102 0302 0102 010c fe08 0510  ................
+00003af0: 010a 0108 0102 800c 0210 010a 010a 020a  ................
+00003b00: 0108 020c 040c 0110 010e 0206 0108 0106  ................
+00003b10: fe0e 0512 0102 0102 0106 0106 fd14 050a  ................
+00003b20: 0114 010c 0308 010e 0102 0106 0106 fe06  ................
+00003b30: 0408 020e 0208 0204 fe10 0308 0304 fd0a  ................
+00003b40: 0312 0306 0104 ff02 ff0a 0404 800c 0206  ................
+00003b50: 0312 010c 010a 020e 020a 0108 0212 0110  ................
+00003b60: 020c 0216 0108 020c 0206 020e 010c 0206  ................
+00003b70: 020a 0108 0108 0206 0102 0204 0104 ff02  ................
+00003b80: ff0a 0404 020c 0102 ff02 0202 fe02 0204  ................
+00003b90: 0210 0102 fe04 ff10 070c 0204 027a 1d41  .............z.A
+00003ba0: 7267 756d 656e 7450 6172 7365 722e 5f61  rgumentParser._a
+00003bb0: 6464 5f61 7267 756d 656e 7473 da01 7463  dd_arguments..tc
+00003bc0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00003bd0: 0400 0000 4300 0000 730c 0000 0074 007c  ....C...s....t.|
+00003be0: 0064 0164 0083 0353 0029 024e da0a 5f5f  .d.d...S.).N..__
+00003bf0: 6f72 6967 696e 5f5f a901 72d7 0000 00a9  origin__..r.....
+00003c00: 0172 e100 0000 7253 0000 0072 5300 0000  .r....rS...rS...
+00003c10: 7257 0000 0072 c500 0000 ba02 0000 f302  rW...r..........
+00003c20: 0000 000c 027a 1f41 7267 756d 656e 7450  .....z.ArgumentP
+00003c30: 6172 7365 722e 5f67 6574 5f74 7970 655f  arser._get_type_
+00003c40: 6f72 6967 696e 6301 0000 0000 0000 0000  originc.........
+00003c50: 0000 0001 0000 0004 0000 0043 0000 00f3  ...........C....
+00003c60: 0c00 0000 7400 7c00 6401 6402 8303 5300  ....t.|.d.d...S.
+00003c70: 2903 4eda 085f 5f61 7267 735f 5f72 5300  ).N..__args__rS.
+00003c80: 0000 72e3 0000 0072 e400 0000 7253 0000  ..r....r....rS..
+00003c90: 0072 5300 0000 7257 0000 0072 cb00 0000  .rS...rW...r....
+00003ca0: be02 0000 72e5 0000 007a 1d41 7267 756d  ....r....z.Argum
+00003cb0: 656e 7450 6172 7365 722e 5f67 6574 5f74  entParser._get_t
+00003cc0: 7970 655f 6172 6773 6301 0000 0000 0000  ype_argsc.......
+00003cd0: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00003ce0: 0072 e600 0000 2903 4eda 0c5f 5f6d 6574  .r....).N..__met
+00003cf0: 6164 6174 615f 5f72 5300 0000 72e3 0000  adata__rS...r...
+00003d00: 0072 e400 0000 7253 0000 0072 5300 0000  .r....rS...rS...
+00003d10: 7257 0000 0072 c700 0000 c202 0000 72e5  rW...r........r.
+00003d20: 0000 007a 2141 7267 756d 656e 7450 6172  ...z!ArgumentPar
+00003d30: 7365 722e 5f67 6574 5f74 7970 655f 6d65  ser._get_type_me
+00003d40: 7461 6461 7461 da0e 7479 7065 5f63 6f6e  tadata..type_con
+00003d50: 7461 696e 6572 72b0 0000 0072 ab00 0000  tainerr....r....
+00003d60: 6304 0000 0000 0000 0000 0000 000b 0000  c...............
+00003d70: 0003 0000 0043 0000 0073 1801 0000 7c03  .....C...s....|.
+00003d80: 7204 7400 6e04 7c00 a001 7c01 a101 7d04  r.t.n.|...|...}.
+00003d90: 7c04 6400 7500 7215 7402 6401 7c01 6a03  |.d.u.r.t.d.|.j.
+00003da0: 9b00 9d02 8301 8201 7c00 a004 7c01 a101  ........|...|...
+00003db0: 7d05 6402 6403 8400 7c05 4400 8301 7d06  }.d.d...|.D...}.
+00003dc0: 7c04 7400 7500 7330 7405 7c04 7406 6a07  |.t.u.s0t.|.t.j.
+00003dd0: 6a08 8302 7330 7c04 7409 7500 7240 740a  j...s0|.t.u.r@t.
+00003de0: 7c06 8301 6404 6b03 723b 7c06 a00b a100  |...d.k.r;|.....
+00003df0: 0100 6e2c 7c06 6405 1900 7d07 6e27 7405  ..n,|.d...}.n't.
+00003e00: 7c04 7406 6a07 6a0c 8302 7261 740a 7c06  |.t.j.j...rat.|.
+00003e10: 8301 6406 6b03 7252 7c06 a00b a100 0100  ..d.k.rR|.......
+00003e20: 6e15 7c06 5c02 7d08 7d09 7c08 740d 7501  n.|.\.}.}.|.t.u.
+00003e30: 725e 7402 6407 8301 8201 7c09 7d07 6e06  r^t.d.....|.}.n.
+00003e40: 740e 7367 740f 7c01 8301 0100 7c06 736d  t.sgt.|.....|.sm
+00003e50: 7402 6408 8301 8201 7c00 a001 7c07 a101  t.d.....|...|...
+00003e60: 7d0a 7c0a 7400 7500 7280 7c00 a010 7c07  }.|.t.u.r.|...|.
+00003e70: a101 7d07 7c00 a001 7c07 a101 7d0a 7c02  ..}.|...|...}.|.
+00003e80: 728a 7c0a 728a 740e 738a 740f 7c0a 8301  r.|.r.t.s.t.|...
+00003e90: 0100 7c07 5300 2909 4e7a 1f47 6976 656e  ..|.S.).Nz.Given
+00003ea0: 2074 7970 6520 6973 206e 6f74 2061 2063   type is not a c
+00003eb0: 6f6e 7461 696e 6572 3a20 6301 0000 0000  ontainer: c.....
+00003ec0: 0000 0000 0000 0002 0000 0004 0000 0053  ...............S
+00003ed0: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
+00003ee0: 7c01 6400 7501 7202 7c01 7400 7501 7202  |.d.u.r.|.t.u.r.
+00003ef0: 7c01 9102 7102 5300 2901 2e29 0172 2b00  |...q.S.)..).r+.
+00003f00: 0000 2902 7255 0000 00da 0161 7253 0000  ..).rU.....arS..
+00003f10: 0072 5300 0000 7257 0000 0072 5800 0000  .rS...rW...rX...
+00003f20: d802 0000 7304 0000 0006 001a 017a 3f41  ....s........z?A
+00003f30: 7267 756d 656e 7450 6172 7365 722e 5f65  rgumentParser._e
+00003f40: 7874 7261 6374 5f74 7970 655f 6672 6f6d  xtract_type_from
+00003f50: 5f63 6f6e 7461 696e 6572 2e3c 6c6f 6361  _container.<loca
+00003f60: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 7217  ls>.<listcomp>r.
+00003f70: 0000 0072 0100 0000 727c 0000 007a 2244  ...r....r|...z"D
+00003f80: 6963 7469 6f6e 6172 7920 6b65 7973 206d  ictionary keys m
+00003f90: 7573 7420 6265 2074 7970 6520 6073 7472  ust be type `str
+00003fa0: 607a 1b54 6f6f 206d 616e 7920 7479 7065  `z.Too many type
+00003fb0: 7320 696e 2063 6f6e 7461 696e 6572 2911  s in container).
+00003fc0: 7215 0000 0072 c500 0000 da09 5479 7065  r....r......Type
+00003fd0: 4572 726f 7272 9500 0000 72cb 0000 0072  Errorr....r....r
+00003fe0: 3900 0000 72cc 0000 0072 cd00 0000 7211  9...r....r....r.
+00003ff0: 0000 0072 d000 0000 7276 0000 00da 0563  ...r....rv.....c
+00004000: 6c65 6172 72ce 0000 0072 6e00 0000 7235  learr....rn...r5
+00004010: 0000 0072 2700 0000 72c6 0000 0029 0b72  ...r'...r....).r
+00004020: a700 0000 72e9 0000 0072 b000 0000 72ab  ....r....r....r.
+00004030: 0000 005a 1574 7970 655f 636f 6e74 6169  ...Z.type_contai
+00004040: 6e65 725f 6f72 6967 696e 5a13 7479 7065  ner_originZ.type
+00004050: 5f63 6f6e 7461 696e 6572 5f61 7267 73da  _container_args.
+00004060: 0772 6573 756c 7473 5a16 7479 7065 5f63  .resultsZ.type_c
+00004070: 6f6e 7461 696e 6572 5f73 7562 7479 7065  ontainer_subtype
+00004080: 5a08 6b65 795f 7479 7065 5a0a 7661 6c75  Z.key_typeZ.valu
+00004090: 655f 7479 7065 5a1d 7479 7065 5f63 6f6e  e_typeZ.type_con
+000040a0: 7461 696e 6572 5f73 7562 7479 7065 5f6f  tainer_subtype_o
+000040b0: 7269 6769 6e72 5300 0000 7253 0000 0072  riginrS...rS...r
+000040c0: 5700 0000 72c6 0000 00c6 0200 0073 5400  W...r........sT.
+000040d0: 0000 1008 02ff 0804 0201 0a01 04ff 0a04  ................
+000040e0: 0602 0201 06ff 0807 0c01 02ff 0802 0c02  ................
+000040f0: 0a01 0a02 0e01 0c01 0a01 0802 0801 0801  ................
+00004100: 0601 0401 0801 0402 0801 0a02 0802 0401  ................
+00004110: 0201 04ff 0a03 0203 02ff 0202 02fe 0203  ................
+00004120: 02fd 0805 0402 7a2b 4172 6775 6d65 6e74  ......z+Argument
+00004130: 5061 7273 6572 2e5f 6578 7472 6163 745f  Parser._extract_
+00004140: 7479 7065 5f66 726f 6d5f 636f 6e74 6169  type_from_contai
+00004150: 6e65 7263 0100 0000 0000 0000 0000 0000  nerc............
+00004160: 0200 0000 0400 0000 4300 0000 7324 0000  ........C...s$..
+00004170: 007c 006a 0044 005d 0c7d 0174 017c 0174  .|.j.D.].}.t.|.t
+00004180: 026a 0383 0272 0f7c 0102 0001 0053 0071  .j...r.|.....S.q
+00004190: 0364 0053 0072 5c00 0000 2904 da08 5f61  .d.S.r\...)..._a
+000041a0: 6374 696f 6e73 726d 0000 0072 7400 0000  ctionsrm...rt...
+000041b0: 7296 0000 0029 0272 7800 0000 72ea 0000  r....).rx...r...
+000041c0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+000041d0: 728c 0000 0006 0300 0073 1000 0000 0a01  r........s......
+000041e0: 0201 0201 0401 04fe 0804 02fc 0405 7a26  ..............z&
+000041f0: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+00004200: 6669 6e64 5f73 7562 7061 7273 6572 735f  find_subparsers_
+00004210: 6163 7469 6f6e 6301 0000 0000 0000 0000  actionc.........
+00004220: 0000 0001 0000 0007 0000 0003 0000 0073  ...............s
+00004230: 4400 0000 8800 6a00 6400 7500 721f 8800  D.....j.d.u.r...
+00004240: 6a01 7210 8800 a002 a100 8800 5f00 8800  j.r........._...
+00004250: 6a00 5300 8800 6a03 6401 6402 8800 6a04  j.S...j.d.d...j.
+00004260: 8700 6601 6403 6404 8408 6405 8d04 8800  ..f.d.d...d.....
+00004270: 5f00 8800 6a00 5300 2906 4e5a 0863 6f6d  _...j.S.).NZ.com
+00004280: 6d61 6e64 737a 093c 434f 4d4d 414e 443e  mandsz.<COMMAND>
+00004290: 6300 0000 0000 0000 0000 0000 0001 0000  c...............
+000042a0: 0006 0000 001b 0000 0073 1e00 0000 7400  .........s....t.
+000042b0: 8800 8301 6403 6900 7c00 a401 6401 8800  ....d.i.|...d...
+000042c0: 6a01 6402 9c02 a401 8e01 5300 2904 4e54  j.d.......S.).NT
+000042d0: 2902 724f 0000 0072 4e00 0000 7253 0000  ).rO...rN...rS..
+000042e0: 0029 0272 ba00 0000 724e 0000 0029 0172  .).r....rN...).r
+000042f0: df00 0000 a901 7278 0000 0072 5300 0000  ......rx...rS...
+00004300: 7257 0000 0072 5e00 0000 1803 0000 730c  rW...r^.......s.
+00004310: 0000 000a 0002 0102 ff02 0204 010a fd7a  ...............z
+00004320: 3741 7267 756d 656e 7450 6172 7365 722e  7ArgumentParser.
+00004330: 5f67 6574 5f6f 725f 6164 645f 7375 6270  _get_or_add_subp
+00004340: 6172 7365 7273 2e3c 6c6f 6361 6c73 3e2e  arsers.<locals>.
+00004350: 3c6c 616d 6264 613e 2904 726c 0000 0072  <lambda>).rl...r
+00004360: b300 0000 72b5 0000 00da 0c70 6172 7365  ....r......parse
+00004370: 725f 636c 6173 7329 0572 6a00 0000 728b  r_class).rj...r.
+00004380: 0000 0072 8c00 0000 da0e 6164 645f 7375  ...r......add_su
+00004390: 6270 6172 7365 7273 7244 0000 0072 ef00  bparsersrD...r..
+000043a0: 0000 7253 0000 0072 ef00 0000 7257 0000  ..rS...r....rW..
+000043b0: 0072 7700 0000 0f03 0000 7316 0000 000a  .rw.......s.....
+000043c0: 0106 010a 0106 0d04 f502 0102 0104 010a  ................
+000043d0: 0108 fc06 0b7a 2541 7267 756d 656e 7450  .....z%ArgumentP
+000043e0: 6172 7365 722e 5f67 6574 5f6f 725f 6164  arser._get_or_ad
+000043f0: 645f 7375 6270 6172 7365 7273 72bd 0000  d_subparsersr...
+00004400: 0063 0200 0000 0000 0000 0000 0000 0600  .c..............
+00004410: 0000 0600 0000 0300 0000 736e 0000 007c  ..........sn...|
+00004420: 006a 00a0 0174 0288 007c 006a 0364 0083  .j...t...|.j.d..
+00004430: 0369 00a1 027d 027c 02a0 04a1 0044 005d  .i...}.|.....D.]
+00004440: 1d7d 0387 0066 0164 0164 0284 087c 0344  .}...f.d.d...|.D
+00004450: 0083 017d 0474 057c 0483 0164 036b 0472  ...}.t.|...d.k.r
+00004460: 2d64 0464 05a0 067c 04a1 0117 007d 057c  -d.d...|.....}.|
+00004470: 00a0 077c 05a1 0101 0071 1074 0864 0669  ...|.....q.t.d.i
+00004480: 0074 0988 0083 01a4 018e 0153 0029 074e  .t.........S.).N
+00004490: 6301 0000 0000 0000 0000 0000 0004 0000  c...............
+000044a0: 0005 0000 0013 0000 0073 6c00 0000 6700  .........sl...g.
+000044b0: 7c00 5d32 5c02 7d01 7d02 7400 8800 7c01  |.]2\.}.}.t...|.
+000044c0: 8302 7234 7401 8800 7c01 8302 7d03 7402  ..r4t...|...}.t.
+000044d0: 7c03 7403 8302 731c 7402 7c03 7404 6a05  |.t...s.t.|.t.j.
+000044e0: 6a06 8302 7320 7c03 6400 7501 732e 7402  j...s |.d.u.s.t.
+000044f0: 7c03 7403 8302 7302 7402 7c03 7404 6a05  |.t...s.t.|.t.j.
+00004500: 6a06 8302 7202 7c03 7202 7c02 7232 7c02  j...r.|.r.|.r2|.
+00004510: 6e01 7c01 9102 7102 5300 725c 0000 0029  n.|...q.S.r\...)
+00004520: 07da 0768 6173 6174 7472 72d7 0000 0072  ...hasattrr....r
+00004530: 3800 0000 726e 0000 0072 cc00 0000 72cd  8...rn...r....r.
+00004540: 0000 0072 cf00 0000 2904 7255 0000 0072  ...r....).rU...r
+00004550: b500 0000 da04 666c 6167 5a0a 6174 7472  ......flagZ.attr
+00004560: 5f76 616c 7565 a901 72bd 0000 0072 5300  _value..r....rS.
+00004570: 0000 7257 0000 0072 5800 0000 3003 0000  ..rW...rX...0...
+00004580: 7330 0000 0006 0006 0208 0102 fd0a 0408  s0..............
+00004590: 0302 f902 0802 0106 0102 fe02 f808 0d08  ................
+000045a0: 0302 fd02 0402 0106 0102 fe02 fc02 0802  ................
+000045b0: f80a f406 0c7a 3341 7267 756d 656e 7450  .....z3ArgumentP
+000045c0: 6172 7365 722e 5f70 6f73 745f 7061 7273  arser._post_pars
+000045d0: 655f 6172 6773 2e3c 6c6f 6361 6c73 3e2e  e_args.<locals>.
+000045e0: 3c6c 6973 7463 6f6d 703e 7217 0000 007a  <listcomp>r....z
+000045f0: 2854 6865 7365 2061 7267 756d 656e 7473  (These arguments
+00004600: 2061 7265 206d 7574 7561 6c6c 7920 6578   are mutually ex
+00004610: 636c 7573 6976 653a 2072 c000 0000 7253  clusive: r....rS
+00004620: 0000 0029 0a72 7100 0000 72aa 0000 0072  ...).rq...r....r
+00004630: d700 0000 7245 0000 0072 be00 0000 7276  ....rE...r....rv
+00004640: 0000 0072 da00 0000 7282 0000 0072 2800  ...r....r....r(.
+00004650: 0000 da04 7661 7273 2906 7278 0000 0072  ....vars).rx...r
+00004660: bd00 0000 5a12 6675 6e63 5f6d 785f 6172  ....Z.func_mx_ar
+00004670: 675f 6772 6f75 7073 5a06 675f 6172 6773  g_groupsZ.g_args
+00004680: 5a0e 6d78 5f66 6c61 6773 5f66 6f75 6e64  Z.mx_flags_found
+00004690: 72dd 0000 0072 5300 0000 72f4 0000 0072  r....rS...r....r
+000046a0: 5700 0000 da10 5f70 6f73 745f 7061 7273  W....._post_pars
+000046b0: 655f 6172 6773 2103 0000 7320 0000 0006  e_args!...s ....
+000046c0: 070c 0102 0102 fe02 fd0c 070a 0402 0206  ................
+000046d0: fe0c 1906 0102 0106 ff0a 0302 8012 027a  ...............z
+000046e0: 1f41 7267 756d 656e 7450 6172 7365 722e  .ArgumentParser.
+000046f0: 5f70 6f73 745f 7061 7273 655f 6172 6773  _post_parse_args
+00004700: 6303 0000 0000 0000 0000 0000 0005 0000  c...............
+00004710: 000a 0000 0003 0000 0073 5200 0000 7a0e  .........sR...z.
+00004720: 7400 8300 6a01 7c01 7c02 6401 8d02 7d03  t...j.|.|.d...}.
+00004730: 7c00 a002 7c03 a101 5700 5300 0400 7403  |...|...W.S...t.
+00004740: 7928 0100 7d04 0100 7a0e 7c00 a004 7405  y(..}...z.|...t.
+00004750: 7c04 8301 a101 0100 5700 5900 6400 7d04  |.......W.Y.d.}.
+00004760: 7e04 6400 5300 6400 7d04 7e04 7701 7700  ~.d.S.d.}.~.w.w.
+00004770: a902 4e29 0272 5000 0000 72bd 0000 0029  ..N).rP...r....)
+00004780: 0672 6800 0000 da0a 7061 7273 655f 6172  .rh.....parse_ar
+00004790: 6773 72f6 0000 00da 0a56 616c 7565 4572  gsr......ValueEr
+000047a0: 726f 7272 8200 0000 726e 0000 0029 0572  rorr....rn...).r
+000047b0: 7800 0000 7250 0000 0072 bd00 0000 da06  x...rP...r......
+000047c0: 7061 7273 6564 da01 6572 7900 0000 7253  parsed..ery...rS
+000047d0: 0000 0072 5700 0000 72f8 0000 0051 0300  ...rW...r....Q..
+000047e0: 0073 1400 0000 0205 0601 0201 0201 06fe  .s..............
+000047f0: 0c04 0e01 1c01 0880 02ff 7a19 4172 6775  ..........z.Argu
+00004800: 6d65 6e74 5061 7273 6572 2e70 6172 7365  mentParser.parse
+00004810: 5f61 7267 7363 0300 0000 0000 0000 0000  _argsc..........
+00004820: 0000 0600 0000 0a00 0000 0300 0000 735a  ..............sZ
+00004830: 0000 007a 1274 0083 006a 017c 017c 0264  ...z.t...j.|.|.d
+00004840: 018d 025c 027d 037d 047c 00a0 027c 03a1  ...\.}.}.|...|..
+00004850: 017c 0466 0257 0053 0004 0074 0379 2c01  .|.f.W.S...t.y,.
+00004860: 007d 0501 007a 0e7c 00a0 0474 057c 0583  .}...z.|...t.|..
+00004870: 01a1 0101 0057 0059 0064 007d 057e 0564  .....W.Y.d.}.~.d
+00004880: 0053 0064 007d 057e 0577 0177 0072 f700  .S.d.}.~.w.w.r..
+00004890: 0000 2906 7268 0000 00da 1070 6172 7365  ..).rh.....parse
+000048a0: 5f6b 6e6f 776e 5f61 7267 7372 f600 0000  _known_argsr....
+000048b0: 72f9 0000 0072 8200 0000 726e 0000 0029  r....r....rn...)
+000048c0: 0672 7800 0000 7250 0000 0072 bd00 0000  .rx...rP...r....
+000048d0: 72fa 0000 00da 0775 6e6b 6e6f 776e 72fb  r......unknownr.
+000048e0: 0000 0072 7900 0000 7253 0000 0072 5700  ...ry...rS...rW.
+000048f0: 0000 72fc 0000 005f 0300 0073 0e00 0000  ..r...._...s....
+00004900: 0207 1401 1001 0e01 1c01 0880 02ff 7a1f  ..............z.
+00004910: 4172 6775 6d65 6e74 5061 7273 6572 2e70  ArgumentParser.p
+00004920: 6172 7365 5f6b 6e6f 776e 5f61 7267 73da  arse_known_args.
+00004930: 1873 6b69 705f 7079 6461 6e74 6963 5f76  .skip_pydantic_v
+00004940: 616c 6964 6174 696f 6e63 0400 0000 0000  alidationc......
+00004950: 0000 0000 0000 0600 0000 0500 0000 4300  ..............C.
+00004960: 0000 7322 0000 007c 00a0 007c 01a1 015c  ..s"...|...|...\
+00004970: 027d 047d 057c 006a 017c 047c 027c 0364  .}.}.|.j.|.|.|.d
+00004980: 018d 037c 0566 0253 0029 0261 c902 0000  ...|.f.S.).a....
+00004990: 5573 6520 7061 7273 6564 2061 7267 7320  Use parsed args 
+000049a0: 746f 2069 6e73 7461 6e74 6961 7465 2074  to instantiate t
+000049b0: 6865 2067 6976 656e 2064 6174 6120 6d6f  he given data mo
+000049c0: 6465 6c2e 0a0a 2020 2020 2020 2020 4172  del...        Ar
+000049d0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+000049e0: 6172 6773 3a0a 2020 2020 2020 2020 2020  args:.          
+000049f0: 2020 6172 6773 5f6d 6f64 656c 3a0a 2020    args_model:.  
+00004a00: 2020 2020 2020 2020 2020 736b 6970 5f70            skip_p
+00004a10: 7964 616e 7469 635f 7661 6c69 6461 7469  ydantic_validati
+00004a20: 6f6e 3a0a 0a20 2020 2020 2020 2045 7861  on:..        Exa
+00004a30: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+00004a40: 2020 203e 3e3e 2069 6d70 6f72 7420 7961     >>> import ya
+00004a50: 7078 0a20 2020 2020 2020 2020 2020 203e  px.            >
+00004a60: 3e3e 2066 726f 6d20 6461 7461 636c 6173  >> from dataclas
+00004a70: 7365 7320 696d 706f 7274 2064 6174 6163  ses import datac
+00004a80: 6c61 7373 0a20 2020 2020 2020 2020 2020  lass.           
+00004a90: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00004aa0: 203e 3e3e 2040 6461 7461 636c 6173 730a   >>> @dataclass.
+00004ab0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00004ac0: 636c 6173 7320 4164 644e 756d 733a 0a20  class AddNums:. 
+00004ad0: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004ae0: 2020 2078 3a20 696e 740a 2020 2020 2020     x: int.      
+00004af0: 2020 2020 2020 2e2e 2e20 2020 2020 793a        ...     y:
+00004b00: 2069 6e74 0a20 2020 2020 2020 2020 2020   int.           
+00004b10: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00004b20: 203e 3e3e 2070 6172 7365 7220 3d20 7961   >>> parser = ya
+00004b30: 7078 2e41 7267 756d 656e 7450 6172 7365  px.ArgumentParse
+00004b40: 7228 290a 2020 2020 2020 2020 2020 2020  r().            
+00004b50: 3e3e 3e20 7061 7273 6572 2e61 6464 5f61  >>> parser.add_a
+00004b60: 7267 756d 656e 7473 2841 6464 4e75 6d73  rguments(AddNums
+00004b70: 290a 2020 2020 2020 2020 2020 2020 3e3e  ).            >>
+00004b80: 3e20 7061 7273 6564 2c20 756e 6b6e 6f77  > parsed, unknow
+00004b90: 6e20 3d20 7061 7273 6572 2e70 6172 7365  n = parser.parse
+00004ba0: 5f6b 6e6f 776e 5f61 7267 735f 746f 5f6d  _known_args_to_m
+00004bb0: 6f64 656c 285b 272d 7827 2c20 2731 272c  odel(['-x', '1',
+00004bc0: 2027 2d79 272c 2027 3227 2c20 272d 7a27   '-y', '2', '-z'
+00004bd0: 2c20 2733 275d 290a 2020 2020 2020 2020  , '3']).        
+00004be0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00004bf0: 2020 2020 3e3e 3e20 2870 6172 7365 642e      >>> (parsed.
+00004c00: 782c 2070 6172 7365 642e 7929 0a20 2020  x, parsed.y).   
+00004c10: 2020 2020 2020 2020 2028 312c 2032 290a           (1, 2).
+00004c20: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00004c30: 756e 6b6e 6f77 6e0a 2020 2020 2020 2020  unknown.        
+00004c40: 2020 2020 5b27 2d7a 272c 2027 3327 5d0a      ['-z', '3'].
+00004c50: 0a20 2020 2020 2020 20a9 0372 5000 0000  .        ..rP...
+00004c60: 728f 0000 0072 fe00 0000 2902 72fc 0000  r....r....).r...
+00004c70: 00da 145f 7061 7273 655f 6172 6773 5f74  ..._parse_args_t
+00004c80: 6f5f 6d6f 6465 6c29 0672 7800 0000 7250  o_model).rx...rP
+00004c90: 0000 0072 8f00 0000 72fe 0000 00da 0b70  ...r....r......p
+00004ca0: 6172 7365 645f 6172 6773 da0c 756e 6b6e  arsed_args..unkn
+00004cb0: 6f77 6e5f 6172 6773 7253 0000 0072 5300  own_argsrS...rS.
+00004cc0: 0000 7257 0000 00da 1970 6172 7365 5f6b  ..rW.....parse_k
+00004cd0: 6e6f 776e 5f61 7267 735f 746f 5f6d 6f64  nown_args_to_mod
+00004ce0: 656c 6c03 0000 7310 0000 000e 2304 0302  ell...s.....#...
+00004cf0: 0102 0102 0104 fd02 0504 fa7a 2841 7267  ...........z(Arg
+00004d00: 756d 656e 7450 6172 7365 722e 7061 7273  umentParser.pars
+00004d10: 655f 6b6e 6f77 6e5f 6172 6773 5f74 6f5f  e_known_args_to_
+00004d20: 6d6f 6465 6c63 0400 0000 0000 0000 0000  modelc..........
+00004d30: 0000 0500 0000 0500 0000 4300 0000 731a  ..........C...s.
+00004d40: 0000 007c 00a0 007c 01a1 017d 047c 006a  ...|...|...}.|.j
+00004d50: 017c 047c 027c 0364 018d 0353 0029 0261  .|.|.|.d...S.).a
+00004d60: 7f02 0000 5573 6520 7061 7273 6564 2061  ....Use parsed a
+00004d70: 7267 7320 746f 2069 6e73 7461 6e74 6961  rgs to instantia
+00004d80: 7465 2074 6865 2067 6976 656e 2064 6174  te the given dat
+00004d90: 6120 6d6f 6465 6c2e 0a0a 2020 2020 2020  a model...      
+00004da0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00004db0: 2020 2020 6172 6773 3a0a 2020 2020 2020      args:.      
+00004dc0: 2020 2020 2020 6172 6773 5f6d 6f64 656c        args_model
+00004dd0: 3a0a 2020 2020 2020 2020 2020 2020 736b  :.            sk
+00004de0: 6970 5f70 7964 616e 7469 635f 7661 6c69  ip_pydantic_vali
+00004df0: 6461 7469 6f6e 3a0a 0a20 2020 2020 2020  dation:..       
+00004e00: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+00004e10: 2020 2020 2020 203e 3e3e 2069 6d70 6f72         >>> impor
+00004e20: 7420 7961 7078 0a20 2020 2020 2020 2020  t yapx.         
+00004e30: 2020 203e 3e3e 2066 726f 6d20 6461 7461     >>> from data
+00004e40: 636c 6173 7365 7320 696d 706f 7274 2064  classes import d
+00004e50: 6174 6163 6c61 7373 0a20 2020 2020 2020  ataclass.       
+00004e60: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00004e70: 2020 2020 203e 3e3e 2040 6461 7461 636c       >>> @datacl
+00004e80: 6173 730a 2020 2020 2020 2020 2020 2020  ass.            
+00004e90: 2e2e 2e20 636c 6173 7320 4164 644e 756d  ... class AddNum
+00004ea0: 733a 0a20 2020 2020 2020 2020 2020 202e  s:.            .
+00004eb0: 2e2e 2020 2020 2078 3a20 696e 740a 2020  ..     x: int.  
+00004ec0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004ed0: 2020 793a 2069 6e74 0a20 2020 2020 2020    y: int.       
+00004ee0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00004ef0: 2020 2020 203e 3e3e 2070 6172 7365 7220       >>> parser 
+00004f00: 3d20 7961 7078 2e41 7267 756d 656e 7450  = yapx.ArgumentP
+00004f10: 6172 7365 7228 290a 2020 2020 2020 2020  arser().        
+00004f20: 2020 2020 3e3e 3e20 7061 7273 6572 2e61      >>> parser.a
+00004f30: 6464 5f61 7267 756d 656e 7473 2841 6464  dd_arguments(Add
+00004f40: 4e75 6d73 290a 2020 2020 2020 2020 2020  Nums).          
+00004f50: 2020 3e3e 3e20 7061 7273 6564 203d 2070    >>> parsed = p
+00004f60: 6172 7365 722e 7061 7273 655f 6172 6773  arser.parse_args
+00004f70: 5f74 6f5f 6d6f 6465 6c28 5b27 2d78 272c  _to_model(['-x',
+00004f80: 2027 3127 2c20 272d 7927 2c20 2732 275d   '1', '-y', '2']
+00004f90: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
+00004fa0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+00004fb0: 3e20 2870 6172 7365 642e 782c 2070 6172  > (parsed.x, par
+00004fc0: 7365 642e 7929 0a20 2020 2020 2020 2020  sed.y).         
+00004fd0: 2020 2028 312c 2032 290a 0a20 2020 2020     (1, 2)..     
+00004fe0: 2020 2072 ff00 0000 2902 72f8 0000 0072     r....).r....r
+00004ff0: 0001 0000 2905 7278 0000 0072 5000 0000  ....).rx...rP...
+00005000: 728f 0000 0072 fe00 0000 7201 0100 0072  r....r....r....r
+00005010: 5300 0000 7253 0000 0072 5700 0000 da13  S...rS...rW.....
+00005020: 7061 7273 655f 6172 6773 5f74 6f5f 6d6f  parse_args_to_mo
+00005030: 6465 6c9a 0300 0073 0c00 0000 0a1e 0401  del....s........
+00005040: 0201 0201 0201 06fd 7a22 4172 6775 6d65  ........z"Argume
+00005050: 6e74 5061 7273 6572 2e70 6172 7365 5f61  ntParser.parse_a
+00005060: 7267 735f 746f 5f6d 6f64 656c 6304 0000  rgs_to_modelc...
+00005070: 0000 0000 0000 0000 0008 0000 000a 0000  ................
+00005080: 0043 0000 0073 aa00 0000 7400 7c01 8301  .C...s....t.|...
+00005090: 7d04 7c02 7310 7c04 a001 7c00 6a02 a101  }.|.s.|...|.j...
+000050a0: 7d02 7c02 7310 7403 8201 7c00 6a04 7c04  }.|.s.t...|.j.|.
+000050b0: 7c02 6401 8d02 7d05 7405 724e 7c03 734e  |.d...}.t.rN|.sN
+000050c0: 7a0d 7400 7406 7c02 8301 6405 6900 7c05  z.t.t.|...d.i.|.
+000050d0: a401 8e01 8301 7d05 5700 6e25 0400 7407  ......}.W.n%..t.
+000050e0: 794d 0100 7d06 0100 7a19 6402 6402 a008  yM..}...z.d.d...
+000050f0: 6403 6404 8400 7c06 a009 a100 4400 8301  d.d...|.....D...
+00005100: a101 1700 7d07 7c00 a00a 7c07 a101 0100  ....}.|...|.....
+00005110: 5700 5900 6400 7d06 7e06 6e05 6400 7d06  W.Y.d.}.~.n.d.}.
+00005120: 7e06 7701 7700 7c02 6405 6900 7c05 a401  ~.w.w.|.d.i.|...
+00005130: 8e01 5300 2906 4ea9 02da 0961 7267 735f  ..S.).N....args_
+00005140: 6469 6374 728f 0000 0072 7d00 0000 6301  dictr....r}...c.
+00005150: 0000 0000 0000 0000 0000 0002 0000 0006  ................
+00005160: 0000 0073 0000 0073 2e00 0000 8100 7c00  ...s...s......|.
+00005170: 5d12 7d01 6400 7c01 6401 1900 6402 1900  ].}.d.|.d...d...
+00005180: 9b00 6403 7c01 6404 1900 9b00 6405 9d05  ..d.|.d.....d...
+00005190: 5600 0100 7102 6406 5300 2907 7a18 4572  V...q.d.S.).z.Er
+000051a0: 726f 7220 7061 7273 696e 6720 6172 6775  ror parsing argu
+000051b0: 6d65 6e74 2060 da03 6c6f 6372 0100 0000  ment `..locr....
+000051c0: 7a03 603b 20da 036d 7367 72ac 0000 004e  z.`; ..msgr....N
+000051d0: 7253 0000 0072 5400 0000 7253 0000 0072  rS...rT...rS...r
+000051e0: 5300 0000 7257 0000 00da 093c 6765 6e65  S...rW.....<gene
+000051f0: 7870 723e d803 0000 730a 0000 0002 8004  xpr>....s.......
+00005200: 0002 021c ff0a ff7a 3641 7267 756d 656e  .......z6Argumen
+00005210: 7450 6172 7365 722e 5f70 6172 7365 5f61  tParser._parse_a
+00005220: 7267 735f 746f 5f6d 6f64 656c 2e3c 6c6f  rgs_to_model.<lo
+00005230: 6361 6c73 3e2e 3c67 656e 6578 7072 3e72  cals>.<genexpr>r
+00005240: 5300 0000 290b 72f5 0000 0072 aa00 0000  S...).r....r....
+00005250: 7246 0000 0072 2600 0000 da16 5f75 6e69  rF...r&....._uni
+00005260: 6f6e 5f61 7267 735f 7769 7468 5f6d 6f64  on_args_with_mod
+00005270: 656c 7235 0000 0072 3300 0000 722e 0000  elr5...r3...r...
+00005280: 0072 da00 0000 da06 6572 726f 7273 7282  .r......errorsr.
+00005290: 0000 0029 0872 7800 0000 7250 0000 0072  ...).rx...rP...r
+000052a0: 8f00 0000 72fe 0000 0072 0101 0000 5a0a  ....r....r....Z.
+000052b0: 6172 6773 5f75 6e69 6f6e 72fb 0000 0072  args_unionr....r
+000052c0: dd00 0000 7253 0000 0072 5300 0000 7257  ....rS...rS...rW
+000052d0: 0000 0072 0001 0000 bf03 0000 732c 0000  ...r........s,..
+000052e0: 0008 0604 020c 0104 0104 0104 0202 0102  ................
+000052f0: 0106 fe08 0502 0202 0110 0108 ff0e 030c  ................
+00005300: 0106 020a fe16 0408 8002 fb0e 077a 2341  .............z#A
+00005310: 7267 756d 656e 7450 6172 7365 722e 5f70  rgumentParser._p
+00005320: 6172 7365 5f61 7267 735f 746f 5f6d 6f64  arse_args_to_mod
+00005330: 656c 7206 0100 0063 0200 0000 0000 0000  elr....c........
+00005340: 0000 0000 0200 0000 0300 0000 0300 0000  ................
+00005350: 7316 0000 0087 0066 0164 0164 0284 087c  s......f.d.d...|
+00005360: 00a0 00a1 0044 0083 0153 0029 034e 6301  .....D...S.).Nc.
+00005370: 0000 0000 0000 0000 0000 0003 0000 0004  ................
+00005380: 0000 0013 0000 0073 2000 0000 6900 7c00  .......s ...i.|.
+00005390: 5d0c 5c02 7d01 7d02 7c01 8800 6a00 7600  ].\.}.}.|...j.v.
+000053a0: 7202 7c01 7c02 9302 7102 5300 7253 0000  r.|.|...q.S.rS..
+000053b0: 0072 a100 0000 a903 7255 0000 0072 df00  .r......rU...r..
+000053c0: 0000 da01 7672 9400 0000 7253 0000 0072  ....vr....rS...r
+000053d0: 5700 0000 da0a 3c64 6963 7463 6f6d 703e  W.....<dictcomp>
+000053e0: e503 0000 7261 0000 007a 3941 7267 756d  ....ra...z9Argum
+000053f0: 656e 7450 6172 7365 722e 5f75 6e69 6f6e  entParser._union
+00005400: 5f61 7267 735f 7769 7468 5f6d 6f64 656c  _args_with_model
+00005410: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00005420: 6f6d 703e 2901 728d 0000 0072 0501 0000  omp>).r....r....
+00005430: 7253 0000 0072 9400 0000 7257 0000 0072  rS...r....rW...r
+00005440: 0a01 0000 e003 0000 7302 0000 0016 057a  ........s......z
+00005450: 2541 7267 756d 656e 7450 6172 7365 722e  %ArgumentParser.
+00005460: 5f75 6e69 6f6e 5f61 7267 735f 7769 7468  _union_args_with
+00005470: 5f6d 6f64 656c 6302 0000 0000 0000 0000  _modelc.........
+00005480: 0000 0006 0000 0004 0000 0043 0000 0073  ...........C...s
+00005490: 8000 0000 6400 7d02 7c01 6a00 7215 7c01  ....d.}.|.j.r.|.
+000054a0: 6a00 a001 7c01 6a02 6401 1700 a101 7315  j...|.j.d.....s.
+000054b0: 7c01 6a00 a003 a100 a004 a100 7d02 7c02  |.j.........}.|.
+000054c0: 7319 6400 5300 6402 7d03 7405 7c02 8301  s.d.S.d.}.t.|...
+000054d0: 4400 5d0c 5c02 7d04 7d05 7c05 a003 a100  D.].\.}.}.|.....
+000054e0: 732b 7c04 7d03 0100 6e01 711f 7c03 6402  s+|.}...n.q.|.d.
+000054f0: 6b04 7236 7c02 6400 7c03 8502 1900 7d02  k.r6|.d.|.....}.
+00005500: 6403 a006 6404 6405 8400 7c02 4400 8301  d...d.d...|.D...
+00005510: a101 5300 2906 4efa 0128 7201 0000 0072  ..S.).N..(r....r
+00005520: 7d00 0000 6301 0000 0000 0000 0000 0000  }...c...........
+00005530: 0002 0000 0003 0000 0073 0000 0073 1800  .........s...s..
+00005540: 0000 8100 7c00 5d07 7d01 7c01 a000 a100  ....|.].}.|.....
+00005550: 5600 0100 7102 6400 5300 725c 0000 0029  V...q.d.S.r\...)
+00005560: 01da 0573 7472 6970 7254 0000 0072 5300  ...striprT...rS.
+00005570: 0000 7253 0000 0072 5700 0000 7209 0100  ..rS...rW...r...
+00005580: 00ff 0300 0073 0400 0000 0280 1600 7a41  .....s........zA
+00005590: 4172 6775 6d65 6e74 5061 7273 6572 2e5f  ArgumentParser._
+000055a0: 6765 745f 6465 7363 7269 7074 696f 6e5f  get_description_
+000055b0: 6672 6f6d 5f64 6f63 7374 7269 6e67 2e3c  from_docstring.<
+000055c0: 6c6f 6361 6c73 3e2e 3c67 656e 6578 7072  locals>.<genexpr
+000055d0: 3e29 07da 075f 5f64 6f63 5f5f 7260 0000  >)...__doc__r`..
+000055e0: 0072 9500 0000 7210 0100 0072 9900 0000  .r....r....r....
+000055f0: da09 656e 756d 6572 6174 6572 da00 0000  ..enumerater....
+00005600: 2906 72a7 0000 0072 8f00 0000 5a11 6465  ).r....r....Z.de
+00005610: 7363 7269 7074 696f 6e5f 6c69 6e65 735a  scription_linesZ
+00005620: 1274 6578 745f 626c 6f63 6b5f 656e 6473  .text_block_ends
+00005630: 5f61 74da 0169 da04 6c69 6e65 7253 0000  _at..i..linerS..
+00005640: 0072 5300 0000 7257 0000 0072 9800 0000  .rS...rW...r....
+00005650: e703 0000 7320 0000 0004 050c 0208 0104  ....s ..........
+00005660: ff0e 0304 0204 0104 0210 0108 0104 0104  ................
+00005670: 0102 fe08 040c 0114 027a 2e41 7267 756d  .........z.Argum
+00005680: 656e 7450 6172 7365 722e 5f67 6574 5f64  entParser._get_d
+00005690: 6573 6372 6970 7469 6f6e 5f66 726f 6d5f  escription_from_
+000056a0: 646f 6373 7472 696e 6763 0300 0000 0000  docstringc......
+000056b0: 0000 0000 0000 0400 0000 0300 0000 4300  ..............C.
+000056c0: 0000 731c 0000 007c 00a0 007c 02a1 017d  ..s....|...|...}
+000056d0: 037c 0372 0c7c 037c 015f 0164 0053 0064  .|.r.|.|._.d.S.d
+000056e0: 0053 0072 5c00 0000 2902 7298 0000 0072  .S.r\...).r....r
+000056f0: 4900 0000 2904 72a7 0000 0072 6600 0000  I...).r....rf...
+00005700: 728f 0000 0072 4900 0000 7253 0000 0072  r....rI...rS...r
+00005710: 5300 0000 7257 0000 00da 1f5f 7365 745f  S...rW....._set_
+00005720: 6465 7363 7269 7074 696f 6e5f 6672 6f6d  description_from
+00005730: 5f64 6f63 7374 7269 6e67 0104 0000 7308  _docstring....s.
+00005740: 0000 000a 0604 020a 0104 ff7a 2e41 7267  ...........z.Arg
+00005750: 756d 656e 7450 6172 7365 722e 5f73 6574  umentParser._set
+00005760: 5f64 6573 6372 6970 7469 6f6e 5f66 726f  _description_fro
+00005770: 6d5f 646f 6373 7472 696e 67da 0b6c 696e  m_docstring..lin
+00005780: 6b65 645f 6675 6e63 da0b 7265 6c61 795f  ked_func..relay_
+00005790: 7661 6c75 6563 0700 0000 0000 0000 0000  valuec..........
+000057a0: 0000 1700 0000 0700 0000 0300 0000 73e6  ..............s.
+000057b0: 0100 0067 007d 0769 007d 0864 017d 0964  ...g.}.i.}.d.}.d
+000057c0: 017d 0a64 017d 0b64 017d 0c64 017d 0d74  .}.d.}.d.}.d.}.t
+000057d0: 007c 0283 016a 01a0 02a1 0044 005d 437d  .|...j.....D.]C}
+000057e0: 0e74 037c 0e83 01a0 0464 02a1 0172 2164  .t.|.....d...r!d
+000057f0: 037d 0c71 1574 037c 0e83 01a0 0464 04a1  .}.q.t.|.....d..
+00005800: 0172 2b64 037d 0a71 157c 0e6a 0564 056b  .r+d.}.q.|.j.d.k
+00005810: 0272 3364 037d 0b71 157c 0e6a 0564 066b  .r3d.}.q.|.j.d.k
+00005820: 0272 3b64 037d 0d71 157c 0e6a 0564 076b  .r;d.}.q.|.j.d.k
+00005830: 0272 457c 037c 0864 073c 0071 157c 0e6a  .rE|.|.d.<.q.|.j
+00005840: 0564 086b 0272 4f7c 067c 0864 083c 0071  .d.k.rO|.|.d.<.q
+00005850: 157c 0e6a 0564 096b 0272 5864 037c 0864  .|.j.d.k.rXd.|.d
+00005860: 093c 0071 157c 0a70 607c 0c70 607c 0b70  .<.q.|.p`|.p`|.p
+00005870: 607c 0d7d 097c 0973 737c 0572 7374 0664  `|.}.|.ss|.rst.d
+00005880: 0a64 0b84 0074 007c 0583 016a 01a0 02a1  .d...t.|...j....
+00005890: 0044 0083 0183 017d 097c 0473 7974 077c  .D.....}.|.syt.|
+000058a0: 0283 017d 047c 0972 e17c 016a 087c 037c  ...}.|.r.|.j.|.|
+000058b0: 0464 0c8d 025c 027d 0f7d 107c 0c73 887c  .d...\.}.}.|.s.|
+000058c0: 0d72 d669 0089 007c 0083 007d 117c 1044  .r.i...|...}.|.D
+000058d0: 005d 247d 127c 12a0 0464 0da1 0172 b37c  .]$}.|...d...r.|
+000058e0: 126a 0964 0e64 0f64 108d 0264 1119 007d  .j.d.d.d...d...}
+000058f0: 137c 13a0 0a64 0da1 017d 147c 1472 b37c  .|...d...}.|.r.|
+00005900: 116a 0b7c 1364 1264 0064 0164 138d 0401  .j.|.d.d.d.d....
+00005910: 007c 1388 007c 143c 0071 8f7c 116a 0c7c  .|...|.<.q.|.j.|
+00005920: 1064 148d 015c 027d 157d 1087 0066 0164  .d...\.}.}...f.d
+00005930: 1564 1684 0874 0d7c 1583 01a0 0ea1 0044  .d...t.|.......D
+00005940: 0083 017d 167c 0c72 d07c 08a0 0f7c 16a1  ...}.|.r.|...|..
+00005950: 0101 007c 0d72 d67c 167c 0864 063c 007c  ...|.r.|.|.d.<.|
+00005960: 0a72 da7c 107d 077c 0b72 e07c 107c 0864  .r.|.}.|.r.|.|.d
+00005970: 053c 006e 077c 016a 107c 037c 0464 0c8d  .<.n.|.j.|.|.d..
+00005980: 027d 0f7c 027c 0769 0074 0d7c 0f83 01a4  .}.|.|.i.t.|....
+00005990: 017c 08a4 018e 0153 0029 174e 467a 022a  .|.....S.).NFz.*
+000059a0: 2a54 da01 2ada 0b5f 6578 7472 615f 6172  *T..*.._extra_ar
+000059b0: 6773 da0d 5f65 7874 7261 5f6b 7761 7267  gs.._extra_kwarg
+000059c0: 735a 095f 616c 6c5f 6172 6773 5a0c 5f72  sZ._all_argsZ._r
+000059d0: 656c 6179 5f76 616c 7565 5a10 5f63 616c  elay_valueZ._cal
+000059e0: 6c65 645f 6672 6f6d 5f63 6c69 6301 0000  led_from_clic...
+000059f0: 0000 0000 0000 0000 0002 0000 0004 0000  ................
+00005a00: 0073 0000 0073 2800 0000 8100 7c00 5d0f  .s...s(.....|.].
+00005a10: 7d01 7400 7c01 8301 a001 6400 a101 700f  }.t.|.....d...p.
+00005a20: 7c01 6a02 6401 7600 5600 0100 7102 6402  |.j.d.v.V...q.d.
+00005a30: 5300 2903 7218 0100 0029 0272 1901 0000  S.).r....).r....
+00005a40: 721a 0100 004e 2903 726e 0000 0072 6000  r....N).rn...r`.
+00005a50: 0000 7292 0000 0029 0272 5500 0000 da01  ..r....).rU.....
+00005a60: 7072 5300 0000 7253 0000 0072 5700 0000  prS...rS...rW...
+00005a70: 7209 0100 0036 0400 0073 0a00 0000 0280  r....6...s......
+00005a80: 0400 0202 16ff 0aff 7a2b 4172 6775 6d65  ........z+Argume
+00005a90: 6e74 5061 7273 6572 2e5f 7275 6e5f 6675  ntParser._run_fu
+00005aa0: 6e63 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  nc.<locals>.<gen
+00005ab0: 6578 7072 3e29 0272 5000 0000 728f 0000  expr>).rP...r...
+00005ac0: 0072 6500 0000 725b 0000 0072 1700 0000  .re...r[...r....
+00005ad0: 72ad 0000 0072 0100 0000 72b9 0000 0029  r....r....r....)
+00005ae0: 0372 b800 0000 7263 0000 0072 b700 0000  .r....rc...r....
+00005af0: 2901 7250 0000 0063 0100 0000 0000 0000  ).rP...c........
+00005b00: 0000 0000 0300 0000 0400 0000 1300 0000  ................
+00005b10: 731a 0000 0069 007c 005d 095c 027d 017d  s....i.|.].\.}.}
+00005b20: 0288 007c 0119 007c 0293 0271 0253 0072  ...|...|...q.S.r
+00005b30: 5300 0000 7253 0000 0072 0c01 0000 a901  S...rS...r......
+00005b40: 5a10 756e 6b6e 6f77 6e5f 6e61 6d65 5f6d  Z.unknown_name_m
+00005b50: 6170 7253 0000 0072 5700 0000 720e 0100  aprS...rW...r...
+00005b60: 005a 0400 0073 0600 0000 0600 0e01 06ff  .Z...s..........
+00005b70: 7a2c 4172 6775 6d65 6e74 5061 7273 6572  z,ArgumentParser
+00005b80: 2e5f 7275 6e5f 6675 6e63 2e3c 6c6f 6361  ._run_func.<loca
+00005b90: 6c73 3e2e 3c64 6963 7463 6f6d 703e 2911  ls>.<dictcomp>).
+00005ba0: 7209 0000 00da 0a70 6172 616d 6574 6572  r......parameter
+00005bb0: 7372 be00 0000 726e 0000 0072 6000 0000  sr....rn...r`...
+00005bc0: 7292 0000 00da 0361 6e79 7225 0000 0072  r......anyr%...r
+00005bd0: 0301 0000 da05 7370 6c69 74da 066c 7374  ......split..lst
+00005be0: 7269 7072 6f00 0000 72fc 0000 0072 f500  ripro...r....r..
+00005bf0: 0000 728d 0000 00da 0675 7064 6174 6572  ..r......updater
+00005c00: 0401 0000 2917 72a7 0000 0072 6600 0000  ....).r....rf...
+00005c10: 729c 0000 0072 5000 0000 728f 0000 0072  r....rP...r....r
+00005c20: 1601 0000 7217 0100 005a 0966 756e 635f  ....r....Z.func_
+00005c30: 6172 6773 5a0b 6675 6e63 5f6b 7761 7267  argsZ.func_kwarg
+00005c40: 735a 0d65 7874 7261 5f61 7267 735f 6f6b  sZ.extra_args_ok
+00005c50: 5a0c 6163 6365 7074 735f 6172 6773 5a12  Z.accepts_argsZ.
+00005c60: 6163 6365 7074 735f 6578 7472 615f 6172  accepts_extra_ar
+00005c70: 6773 5a0e 6163 6365 7074 735f 6b77 6172  gsZ.accepts_kwar
+00005c80: 6773 5a14 6163 6365 7074 735f 6578 7472  gsZ.accepts_extr
+00005c90: 615f 6b77 6172 6773 721b 0100 005a 0a6d  a_kwargsr....Z.m
+00005ca0: 6f64 656c 5f69 6e73 7472 0201 0000 5a0e  odel_instr....Z.
+00005cb0: 756e 6b6e 6f77 6e5f 7061 7273 6572 7256  unknown_parserrV
+00005cc0: 0000 005a 0678 5f66 6c61 675a 0b78 5f66  ...Z.x_flagZ.x_f
+00005cd0: 6c61 675f 6261 7265 5a0e 7061 7273 6564  lag_bareZ.parsed
+00005ce0: 5f75 6e6b 6e6f 776e 5a0c 6578 7472 615f  _unknownZ.extra_
+00005cf0: 6b77 6172 6773 7253 0000 0072 1c01 0000  kwargsrS...r....
+00005d00: 7257 0000 00da 095f 7275 6e5f 6675 6e63  rW....._run_func
+00005d10: 0c04 0000 7390 0000 0004 0a04 0104 0204  ....s...........
+00005d20: 0204 0104 0204 0112 020e 0106 010e 0106  ................
+00005d30: 010a 0106 010a 0106 010a 010a 010a 010a  ................
+00005d40: 010a 0108 0102 800e 0302 ff08 0408 010c  ................
+00005d50: 0208 fe04 0508 0104 0304 0202 0102 010a  ................
+00005d60: fe08 0504 0106 0108 010a 0112 010a 0104  ................
+00005d70: 0104 0102 0102 0102 0102 0106 fc08 0602  ................
+00005d80: 8004 0202 010a ff0a 040a 0106 ff04 030a  ................
+00005d90: 0104 0108 0104 0204 0104 0208 0102 8004  ................
+00005da0: 0302 0102 0106 fe16 057a 1841 7267 756d  .........z.Argum
+00005db0: 656e 7450 6172 7365 722e 5f72 756e 5f66  entParser._run_f
+00005dc0: 756e 63da 0763 6f6d 6d61 6e64 da0b 7375  unc..command..su
+00005dd0: 6263 6f6d 6d61 6e64 73da 116e 616d 6564  bcommands..named
+00005de0: 5f73 7562 636f 6d6d 616e 6473 6304 0000  _subcommandsc...
+00005df0: 0000 0000 0000 0000 0009 0000 000b 0000  ................
+00005e00: 004b 0000 0073 d200 0000 7c00 6403 6900  .K...s....|.d.i.
+00005e10: 7c04 a401 8e01 7d05 7c01 722e 7400 7c01  |.....}.|.r.t.|.
+00005e20: 8301 7d06 7c00 6a01 7c05 7c06 6401 8d02  ..}.|.j.|.|.d...
+00005e30: 0100 7c05 a002 7c06 a101 0100 7c05 6a03  ..|...|.....|.j.
+00005e40: 6403 6900 7c00 6a04 7c01 7c00 6a05 7c06  d.i.|.j.|.|.j.|.
+00005e50: 7c00 6a06 7c01 7c00 6a07 7c06 6904 a401  |.j.|.|.j.|.i...
+00005e60: 8e01 0100 6e14 7c05 6a03 6403 6900 7c00  ....n.|.j.d.i.|.
+00005e70: 6a05 6400 7c00 6a04 6400 7c00 6a07 6400  j.d.|.j.d.|.j.d.
+00005e80: 7c00 6a06 6400 6904 a401 8e01 0100 7c02  |.j.d.i.......|.
+00005e90: 7255 7408 7c02 8301 724b 7c02 6701 7d02  rUt.|...rK|.g.}.
+00005ea0: 7c02 4400 5d07 7d07 7c05 a009 7c07 a101  |.D.].}.|...|...
+00005eb0: 0100 714d 7c03 7267 7c03 a00a a100 4400  ..qM|.rg|.....D.
+00005ec0: 5d0b 5c02 7d08 7d07 7c05 6a09 7c07 7c08  ].\.}.}.|.j.|.|.
+00005ed0: 6402 8d02 0100 715b 7c05 5300 2904 4e29  d.....q[|.S.).N)
+00005ee0: 0272 6600 0000 728f 0000 0072 b100 0000  .rf...r....r....
+00005ef0: 7253 0000 0029 0b72 2500 0000 7215 0100  rS...).r%...r...
+00005f00: 0072 9100 0000 729d 0000 0072 4200 0000  .r....r....rB...
+00005f10: 7243 0000 0072 4500 0000 7246 0000 00da  rC...rE...rF....
+00005f20: 0863 616c 6c61 626c 6572 9e00 0000 728d  .callabler....r.
+00005f30: 0000 0029 0972 a700 0000 7223 0100 0072  ...).r....r#...r
+00005f40: 2401 0000 7225 0100 0072 5100 0000 7266  $...r%...rQ...rf
+00005f50: 0000 005a 0e72 6f6f 745f 6172 675f 6d6f  ...Z.root_arg_mo
+00005f60: 6465 6c72 5600 0000 7292 0000 0072 5300  delrV...r....rS.
+00005f70: 0000 7253 0000 0072 5700 0000 da0d 5f62  ..rS...rW....._b
+00005f80: 7569 6c64 5f70 6172 7365 7270 0400 0073  uild_parserp...s
+00005f90: 3e00 0000 0e08 0402 0801 0401 0201 0201  >...............
+00005fa0: 06fe 0a04 0801 0602 0601 0601 0601 02fc  ................
+00005fb0: 08ff 0809 0602 0601 0601 0601 02fc 06ff  ................
+00005fc0: 0409 0801 0601 0801 0c01 0402 1001 1001  ................
+00005fd0: 0402 7a1c 4172 6775 6d65 6e74 5061 7273  ..z.ArgumentPars
+00005fe0: 6572 2e5f 6275 696c 645f 7061 7273 6572  er._build_parser
+00005ff0: 2902 7250 0000 00da 0c64 6566 6175 6c74  ).rP.....default
+00006000: 5f61 7267 73da 0b70 6172 7365 725f 6172  _args..parser_ar
+00006010: 6773 7228 0100 00da 0d70 6172 7365 725f  gsr(.....parser_
+00006020: 6b77 6172 6773 6301 0000 0000 0000 0002  kwargsc.........
+00006030: 0000 0011 0000 0009 0000 004f 0000 0073  ...........O...s
+00006040: 3801 0000 7c00 6a00 7c03 6900 7c04 a401  8...|.j.|.i.|...
+00006050: 8e01 7d05 7c01 6401 7500 7213 7401 6a02  ..}.|.d.u.r.t.j.
+00006060: 6402 6401 8502 1900 7d01 7c01 7319 7c02  d.d.....}.|.s.|.
+00006070: 7219 7c02 7d01 7c05 a003 7c01 a101 5c02  r.|.}.|...|...\.
+00006080: 7d06 7d07 7404 7c06 8301 7d08 7c08 a005  }.}.t.|...}.|...
+00006090: 7c00 6a06 a101 7d09 7c08 a005 7c00 6a07  |.j...}.|...|.j.
+000060a0: a101 7d0a 7c08 a005 7c00 6a08 a101 7d0b  ..}.|...|.j...}.
+000060b0: 7c08 a005 7c00 6a09 a101 7d0c 7c08 a005  |...|.j...}.|...
+000060c0: 7c00 6a0a a101 7d0d 6401 7d0e 6401 7d0f  |.j...}.d.}.d.}.
+000060d0: 7c09 7252 7c00 6a0b 7c05 7c09 7c0a 7c0c  |.rR|.j.|.|.|.|.
+000060e0: 7c01 6403 8d05 7d0f 740c 7c0f 740d 8302  |.d...}.t.|.t...
+000060f0: 7269 7a06 740e 7c0f 8301 7d0e 5700 6e0d  riz.t.|...}.W.n.
+00006100: 0400 740f 7968 0100 0100 0100 7c0f 7d0e  ..t.yh......|.}.
+00006110: 5900 6e03 7700 7c0f 7d0e 7a20 7c0b 727b  Y.n.w.|.}.z |.r{
+00006120: 7c0c 727b 7c00 6a0b 7c05 7c0c 7c0d 7c01  |.r{|.j.|.|.|.|.
+00006130: 7c09 7c0e 6404 8d06 7d0e 5700 740c 7c0f  |.|.d...}.W.t.|.
+00006140: 740d 8302 728a 7c0f 4400 5d06 7d10 7c0c  t...r.|.D.].}.|.
+00006150: 7389 7c10 7d0e 7183 7c0e 5300 740c 7c0f  s.|.}.q.|.S.t.|.
+00006160: 740d 8302 729a 7c0f 4400 5d07 7d10 7c0c  t...r.|.D.].}.|.
+00006170: 7399 7c10 7d0e 7193 7700 7700 2905 612d  s.|.}.q.w.w.).a-
+00006180: 0300 0055 7365 2067 6976 656e 2066 756e  ...Use given fun
+00006190: 6374 696f 6e73 2074 6f20 636f 6e73 7472  ctions to constr
+000061a0: 7563 7420 6120 434c 492c 2070 6172 7365  uct a CLI, parse
+000061b0: 2074 6865 2061 7267 732c 2061 6e64 2069   the args, and i
+000061c0: 6e76 6f6b 6520 7468 6520 6170 7072 6f70  nvoke the approp
+000061d0: 7269 6174 6520 636f 6d6d 616e 642e 0a0a  riate command...
+000061e0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000061f0: 2020 2020 2020 2020 2020 2a70 6172 7365            *parse
+00006200: 725f 6172 6773 3a0a 2020 2020 2020 2020  r_args:.        
+00006210: 2020 2020 6172 6773 3a0a 2020 2020 2020      args:.      
+00006220: 2020 2020 2020 6465 6661 756c 745f 6172        default_ar
+00006230: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00006240: 2a2a 7061 7273 6572 5f6b 7761 7267 733a  **parser_kwargs:
+00006250: 0a0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00006260: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
+00006270: 203e 3e3e 2069 6d70 6f72 7420 7961 7078   >>> import yapx
+00006280: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00006290: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000062a0: 2064 6566 2070 7269 6e74 5f6e 756d 7328   def print_nums(
+000062b0: 2a61 7267 7329 3a0a 2020 2020 2020 2020  *args):.        
+000062c0: 2020 2020 2e2e 2e20 2020 2020 7072 696e      ...     prin
+000062d0: 7428 2741 7267 733a 2027 2c20 2a61 7267  t('Args: ', *arg
+000062e0: 7329 0a20 2020 2020 2020 2020 2020 202e  s).            .
 000062f0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00006300: 3e3e 2064 6566 2066 696e 645f 6f64 6473  >> def find_odds
-00006310: 282a 6172 6773 293a 0a20 2020 2020 2020  (*args):.       
-00006320: 2020 2020 202e 2e2e 2020 2020 2072 6574       ...     ret
-00006330: 7572 6e20 5b78 2066 6f72 2078 2069 6e20  urn [x for x in 
-00006340: 6172 6773 2069 6620 696e 7428 7829 2025  args if int(x) %
-00006350: 2032 2021 3d20 305d 0a20 2020 2020 2020   2 != 0].       
-00006360: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00006370: 2020 2020 203e 3e3e 2063 6c69 5f61 7267       >>> cli_arg
-00006380: 7320 3d20 5b27 6669 6e64 2d6f 6464 7327  s = ['find-odds'
-00006390: 2c20 2731 272c 2027 3227 2c20 2733 272c  , '1', '2', '3',
-000063a0: 2027 3427 2c20 2735 275d 0a20 2020 2020   '4', '5'].     
-000063b0: 2020 2020 2020 203e 3e3e 2079 6170 782e         >>> yapx.
-000063c0: 7275 6e28 7072 696e 745f 6e75 6d73 2c20  run(print_nums, 
-000063d0: 5b66 696e 645f 6576 656e 732c 2066 696e  [find_evens, fin
-000063e0: 645f 6f64 6473 5d2c 2061 7267 733d 636c  d_odds], args=cl
-000063f0: 695f 6172 6773 290a 2020 2020 2020 2020  i_args).        
-00006400: 2020 2020 4172 6773 3a20 2031 2032 2033      Args:  1 2 3
-00006410: 2034 2035 0a20 2020 2020 2020 2020 2020   4 5.           
-00006420: 205b 2731 272c 2027 3327 2c20 2735 275d   ['1', '3', '5']
-00006430: 0a20 2020 2020 2020 204e 7217 0000 0029  .        Nr....)
-00006440: 0572 6600 0000 729b 0000 0072 8d00 0000  .rf...r....r....
-00006450: 7215 0100 0072 5000 0000 2906 7266 0000  r....rP...).rf..
-00006460: 0072 9b00 0000 728d 0000 0072 5000 0000  .r....r....rP...
-00006470: 7215 0100 0072 1601 0000 2910 7226 0100  r....r....).r&..
-00006480: 0072 7d00 0000 da04 6172 6776 72fb 0000  .r}.....argvr...
-00006490: 0072 f400 0000 72a9 0000 0072 4200 0000  .r....r....rB...
-000064a0: 7243 0000 0072 4400 0000 7245 0000 0072  rC...rD...rE...r
-000064b0: 4600 0000 7221 0100 0072 3800 0000 720a  F...r!...r8...r.
-000064c0: 0000 00da 046e 6578 74da 0d53 746f 7049  .....next..StopI
-000064d0: 7465 7261 7469 6f6e 2911 72a6 0000 0072  teration).r....r
-000064e0: 5000 0000 7227 0100 0072 2801 0000 7229  P...r'...r(...r)
-000064f0: 0100 0072 6600 0000 5a0a 6b6e 6f77 6e5f  ...rf...Z.known_
-00006500: 6172 6773 7284 0000 0072 0001 0000 5a09  argsr....r....Z.
-00006510: 726f 6f74 5f66 756e 635a 1472 6f6f 745f  root_funcZ.root_
-00006520: 6675 6e63 5f61 7267 735f 6d6f 6465 6c5a  func_args_modelZ
-00006530: 0c63 6f6d 6d61 6e64 5f6e 616d 655a 0c63  .command_nameZ.c
-00006540: 6f6d 6d61 6e64 5f66 756e 635a 1763 6f6d  ommand_funcZ.com
-00006550: 6d61 6e64 5f66 756e 635f 6172 6773 5f6d  mand_func_args_m
-00006560: 6f64 656c 7216 0100 005a 0b72 6f6f 745f  odelr....Z.root_
-00006570: 7265 7375 6c74 5a0a 6765 6e5f 7265 7375  resultZ.gen_resu
-00006580: 6c74 7253 0000 0072 5300 0000 7257 0000  ltrS...rS...rW..
-00006590: 00da 045f 7275 6e9a 0400 0073 7a00 0000  ..._run....sz...
-000065a0: 1023 0802 0e01 0802 0401 0e03 0801 0402  .#..............
-000065b0: 0401 04ff 0403 0401 04ff 0c03 0401 0401  ................
-000065c0: 04ff 0403 0401 04ff 0404 0401 0402 0401  ................
-000065d0: 0201 0201 0201 0201 0201 06fb 0a08 0201  ................
-000065e0: 0c01 0c01 0801 02ff 0403 0202 0801 0401  ................
-000065f0: 0201 0201 0201 0201 0201 0201 06fa 0280  ................
-00006600: 0a09 0801 0401 0401 0280 0402 0afb 0801  ................
-00006610: 0401 0401 0280 02fd 0201 7a13 4172 6775  ..........z.Argu
-00006620: 6d65 6e74 5061 7273 6572 2e5f 7275 6e29  mentParser._run)
-00006630: 024e 4672 5c00 0000 2902 4646 2902 4e4e  .NFr\...).FF).NN
-00006640: 2903 4e4e 4629 034e 4e4e 2939 7294 0000  ).NNF).NNN)9r...
-00006650: 00da 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  ...__module__.._
-00006660: 5f71 7561 6c6e 616d 655f 5f72 4200 0000  _qualname__rB...
-00006670: 726d 0000 0072 a100 0000 7243 0000 0072  rm...r....rC...r
-00006680: 4400 0000 7245 0000 0072 4600 0000 722d  D...rE...rF...r-
-00006690: 0000 0072 0c00 0000 7210 0000 0072 0f00  ...r....r....r..
-000066a0: 0000 7213 0000 0072 d300 0000 7269 0000  ..r....r....ri..
-000066b0: 0072 8000 0000 720b 0000 0072 8800 0000  .r....r....r....
-000066c0: 7215 0000 0072 0d00 0000 7229 0000 0072  r....r....r)...r
-000066d0: 8f00 0000 7273 0000 0072 4100 0000 729a  ....rs...rA...r.
-000066e0: 0000 0072 9d00 0000 da0c 7374 6174 6963  ...r......static
-000066f0: 6d65 7468 6f64 72a3 0000 00da 0b63 6c61  methodr......cla
-00006700: 7373 6d65 7468 6f64 7222 0000 0072 8e00  ssmethodr"...r..
-00006710: 0000 72c4 0000 0072 1200 0000 72ca 0000  ..r....r....r...
-00006720: 0072 c600 0000 72c5 0000 0072 9500 0000  .r....r....r....
-00006730: 7289 0000 0072 9300 0000 7228 0000 0072  r....r....r(...r
-00006740: f500 0000 7211 0000 0072 f700 0000 72fb  ....r....r....r.
-00006750: 0000 0072 0201 0000 7203 0100 0072 ff00  ...r....r....r..
-00006760: 0000 720e 0000 0072 0901 0000 7297 0000  ..r....r....r...
-00006770: 0072 1401 0000 7221 0100 0072 2601 0000  .r....r!...r&...
-00006780: 722d 0100 00da 0d5f 5f63 6c61 7373 6365  r-.....__classce
-00006790: 6c6c 5f5f 7253 0000 0072 5300 0000 7277  ll__rS...rS...rw
-000067a0: 0000 0072 5700 0000 7241 0000 004c 0000  ...rW...rA...L..
-000067b0: 0073 d201 0000 0a00 0c01 0c01 0c01 0c01  .s..............
-000067c0: 0c01 0205 0201 0201 0201 0201 0201 0201  ................
-000067d0: 0201 0201 06f5 0202 02fe 0603 02fd 0604  ................
-000067e0: 02fc 0605 02fb 0a06 02fa 0a07 02f9 0a08  ................
-000067f0: 02f8 0a09 02f7 060a 02f6 020b 02f5 020c  ................
-00006800: 0ef4 0e6e 0206 0201 04fd 0a02 02fe 0203  ...n............
-00006810: 02fd 0204 0efc 022d 1602 02fe 0203 0afd  .......-........
-00006820: 0234 04fd 1602 02fe 0603 02fd 0204 02fc  .4..............
-00006830: 0405 0afb 0263 04fd 0a02 02fe 0603 02fd  .....c..........
-00006840: 0204 02fc 0205 0afb 020e 1c01 0203 0201  ................
-00006850: 0402 02fe 1603 02fd 0604 0cfc 007f 007f  ................
-00006860: 0222 2001 0203 2401 0203 2401 0203 0204  ." ...$...$.....
-00006870: 0201 04fc 0602 02fe 0203 02fd 0204 02fc  ................
-00006880: 0605 0cfb 143f 1009 0211 0402 02fe 0203  .....?..........
-00006890: 0afd 0232 0201 04fd 0a02 02fe 0803 02fd  ...2............
-000068a0: 0204 0efc 0210 0201 04fd 0a02 02fe 0803  ................
-000068b0: 02fd 0e04 0efc 020f 0201 0201 04fc 0a02  ................
-000068c0: 02fe 0a03 02fd 0204 02fc 0e05 0afb 0230  ...............0
-000068d0: 0201 0201 04fc 0a02 02fe 0a03 02fd 0204  ................
-000068e0: 02fc 0205 0afb 0228 0201 04fc 0402 02fe  .......(........
-000068f0: 0a03 02fd 0204 02fc 0205 0afb 0221 0201  .............!..
-00006900: 0a01 02ff 0602 02fe 0a03 0cfd 0206 0201  ................
-00006910: 1602 02fe 0603 0cfd 0219 0201 0402 02fe  ................
-00006920: 1603 02fd 0204 0cfc 020a 0206 0201 0201  ................
-00006930: 04f9 0202 02fe 0a03 02fd 0604 02fc 0a05  ................
-00006940: 02fb 0e06 02fa 0607 02f9 0208 0cf8 0263  ...............c
-00006950: 0203 0201 0201 04fc 0e02 02fe 1203 02fd  ................
-00006960: 1604 02fc 0205 02fb 0206 0cfa 022e 0204  ................
-00006970: 0201 06fc 0202 02fe 0a03 02fd 0a04 02fc  ................
-00006980: 0205 02fb 0206 14fa 7241 0000 0029 4e72  ........rA...)Nr
-00006990: 7300 0000 da0f 636f 6c6c 6563 7469 6f6e  s.....collection
-000069a0: 732e 6162 6372 cb00 0000 727d 0000 0072  s.abcr....r}...r
-000069b0: 0200 0000 da0a 636f 6e74 6578 746c 6962  ......contextlib
-000069c0: 7203 0000 00da 0b64 6174 6163 6c61 7373  r......dataclass
-000069d0: 6573 7204 0000 0072 0500 0000 7206 0000  esr....r....r...
-000069e0: 00da 0465 6e75 6d72 0700 0000 da09 6675  ...enumr......fu
-000069f0: 6e63 746f 6f6c 7372 0800 0000 da07 696e  nctoolsr......in
-00006a00: 7370 6563 7472 0900 0000 da05 7479 7065  spectr......type
-00006a10: 7372 0a00 0000 da06 7479 7069 6e67 720b  sr......typingr.
-00006a20: 0000 0072 0c00 0000 720d 0000 0072 0e00  ...r....r....r..
-00006a30: 0000 720f 0000 0072 1000 0000 7211 0000  ..r....r....r...
-00006a40: 0072 1200 0000 7213 0000 0072 1400 0000  .r....r....r....
-00006a50: 7215 0000 005a 0d70 6b67 5f72 6573 6f75  r....Z.pkg_resou
-00006a60: 7263 6573 7216 0000 00da 0761 6374 696f  rcesr......actio
-00006a70: 6e73 7218 0000 0072 1900 0000 721a 0000  nsr....r....r...
-00006a80: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00006a90: 721e 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
-00006aa0: 0361 7267 7221 0000 0072 2200 0000 7223  .argr!...r"...r#
-00006ab0: 0000 0072 2400 0000 7225 0000 00da 0a65  ...r$...r%.....e
-00006ac0: 7863 6570 7469 6f6e 7372 2600 0000 7227  xceptionsr&...r'
-00006ad0: 0000 0072 bc00 0000 7228 0000 0072 2900  ...r....r(...r).
-00006ae0: 0000 722a 0000 0072 2b00 0000 da05 7574  ..r*...r+.....ut
-00006af0: 696c 7372 2c00 0000 722d 0000 0072 2e00  ilsr,...r-...r..
-00006b00: 0000 722f 0000 0072 3000 0000 7231 0000  ..r/...r0...r1..
-00006b10: 0072 3200 0000 7233 0000 0072 3400 0000  .r2...r3...r4...
-00006b20: 7235 0000 0072 3600 0000 7237 0000 0072  r5...r6...r7...r
-00006b30: 3800 0000 7239 0000 0072 c300 0000 723c  8...r9...r....r<
-00006b40: 0000 005a 1174 7970 696e 675f 6578 7465  ...Z.typing_exte
-00006b50: 6e73 696f 6e73 723f 0000 0072 4000 0000  nsionsr?...r@...
-00006b60: 7241 0000 0072 5300 0000 7253 0000 0072  rA...rS...rS...r
-00006b70: 5300 0000 7257 0000 00da 083c 6d6f 6475  S...rW.....<modu
-00006b80: 6c65 3e01 0000 0073 3200 0000 0800 0801  le>....s2.......
-00006b90: 0801 0c01 0c01 1401 0c01 0c01 0c01 0c01  ................
-00006ba0: 3401 0c0e 2c02 1c0b 1007 0c01 1401 4001  4...,.........@.
-00006bb0: 0a11 0e01 0c02 0a02 0c01 0802 1603       ..............
+00006300: 3e3e 2064 6566 2066 696e 645f 6576 656e  >> def find_even
+00006310: 7328 2a61 7267 7329 3a0a 2020 2020 2020  s(*args):.      
+00006320: 2020 2020 2020 2e2e 2e20 2020 2020 7265        ...     re
+00006330: 7475 726e 205b 7820 666f 7220 7820 696e  turn [x for x in
+00006340: 2061 7267 7320 6966 2069 6e74 2878 2920   args if int(x) 
+00006350: 2520 3220 3d3d 2030 5d0a 2020 2020 2020  % 2 == 0].      
+00006360: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00006370: 2020 2020 2020 3e3e 3e20 6465 6620 6669        >>> def fi
+00006380: 6e64 5f6f 6464 7328 2a61 7267 7329 3a0a  nd_odds(*args):.
+00006390: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+000063a0: 2020 2020 7265 7475 726e 205b 7820 666f      return [x fo
+000063b0: 7220 7820 696e 2061 7267 7320 6966 2069  r x in args if i
+000063c0: 6e74 2878 2920 2520 3220 213d 2030 5d0a  nt(x) % 2 != 0].
+000063d0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+000063e0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000063f0: 636c 695f 6172 6773 203d 205b 2766 696e  cli_args = ['fin
+00006400: 642d 6f64 6473 272c 2027 3127 2c20 2732  d-odds', '1', '2
+00006410: 272c 2027 3327 2c20 2734 272c 2027 3527  ', '3', '4', '5'
+00006420: 5d0a 2020 2020 2020 2020 2020 2020 3e3e  ].            >>
+00006430: 3e20 7961 7078 2e72 756e 2870 7269 6e74  > yapx.run(print
+00006440: 5f6e 756d 732c 205b 6669 6e64 5f65 7665  _nums, [find_eve
+00006450: 6e73 2c20 6669 6e64 5f6f 6464 735d 2c20  ns, find_odds], 
+00006460: 6172 6773 3d63 6c69 5f61 7267 7329 0a20  args=cli_args). 
+00006470: 2020 2020 2020 2020 2020 2041 7267 733a             Args:
+00006480: 2020 3120 3220 3320 3420 350a 2020 2020    1 2 3 4 5.    
+00006490: 2020 2020 2020 2020 5b27 3127 2c20 2733          ['1', '3
+000064a0: 272c 2027 3527 5d0a 2020 2020 2020 2020  ', '5'].        
+000064b0: 4e72 1700 0000 2905 7266 0000 0072 9c00  Nr....).rf...r..
+000064c0: 0000 728f 0000 0072 1601 0000 7250 0000  ..r....r....rP..
+000064d0: 0029 0672 6600 0000 729c 0000 0072 8f00  .).rf...r....r..
+000064e0: 0000 7250 0000 0072 1601 0000 7217 0100  ..rP...r....r...
+000064f0: 0029 1072 2701 0000 727f 0000 00da 0461  .).r'...r......a
+00006500: 7267 7672 fc00 0000 72f5 0000 0072 aa00  rgvr....r....r..
+00006510: 0000 7242 0000 0072 4300 0000 7244 0000  ..rB...rC...rD..
+00006520: 0072 4500 0000 7246 0000 0072 2201 0000  .rE...rF...r"...
+00006530: 7238 0000 0072 0a00 0000 da04 6e65 7874  r8...r......next
+00006540: da0d 5374 6f70 4974 6572 6174 696f 6e29  ..StopIteration)
+00006550: 1172 a700 0000 7250 0000 0072 2801 0000  .r....rP...r(...
+00006560: 7229 0100 0072 2a01 0000 7266 0000 005a  r)...r*...rf...Z
+00006570: 0a6b 6e6f 776e 5f61 7267 7372 8600 0000  .known_argsr....
+00006580: 7201 0100 005a 0972 6f6f 745f 6675 6e63  r....Z.root_func
+00006590: 5a14 726f 6f74 5f66 756e 635f 6172 6773  Z.root_func_args
+000065a0: 5f6d 6f64 656c 5a0c 636f 6d6d 616e 645f  _modelZ.command_
+000065b0: 6e61 6d65 5a0c 636f 6d6d 616e 645f 6675  nameZ.command_fu
+000065c0: 6e63 5a17 636f 6d6d 616e 645f 6675 6e63  ncZ.command_func
+000065d0: 5f61 7267 735f 6d6f 6465 6c72 1701 0000  _args_modelr....
+000065e0: 5a0b 726f 6f74 5f72 6573 756c 745a 0a67  Z.root_resultZ.g
+000065f0: 656e 5f72 6573 756c 7472 5300 0000 7253  en_resultrS...rS
+00006600: 0000 0072 5700 0000 da04 5f72 756e 9f04  ...rW....._run..
+00006610: 0000 737a 0000 0010 2308 020e 0108 0204  ..sz....#.......
+00006620: 010e 0308 0104 0204 0104 ff04 0304 0104  ................
+00006630: ff0c 0304 0104 0104 ff04 0304 0104 ff04  ................
+00006640: 0404 0104 0204 0102 0102 0102 0102 0102  ................
+00006650: 0106 fb0a 0802 010c 010c 0108 0102 ff04  ................
+00006660: 0302 0208 0104 0102 0102 0102 0102 0102  ................
+00006670: 0102 0106 fa02 800a 0908 0104 0104 0102  ................
+00006680: 8004 020a fb08 0104 0104 0102 8002 fd02  ................
+00006690: 017a 1341 7267 756d 656e 7450 6172 7365  .z.ArgumentParse
+000066a0: 722e 5f72 756e 2902 4e46 725c 0000 0029  r._run).NFr\...)
+000066b0: 0246 4629 024e 4e29 034e 4e46 2903 4e4e  .FF).NN).NNF).NN
+000066c0: 4e29 3972 9500 0000 da0a 5f5f 6d6f 6475  N)9r......__modu
+000066d0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000066e0: 5f5f 7242 0000 0072 6e00 0000 72a2 0000  __rB...rn...r...
+000066f0: 0072 4300 0000 7244 0000 0072 4500 0000  .rC...rD...rE...
+00006700: 7246 0000 0072 2d00 0000 720c 0000 0072  rF...r-...r....r
+00006710: 1000 0000 720f 0000 0072 1300 0000 72d4  ....r....r....r.
+00006720: 0000 0072 6900 0000 7282 0000 0072 0b00  ...ri...r....r..
+00006730: 0000 728a 0000 0072 1500 0000 720d 0000  ..r....r....r...
+00006740: 0072 2900 0000 7291 0000 0072 7400 0000  .r)...r....rt...
+00006750: 7241 0000 0072 9b00 0000 729e 0000 00da  rA...r....r.....
+00006760: 0c73 7461 7469 636d 6574 686f 6472 a400  .staticmethodr..
+00006770: 0000 da0b 636c 6173 736d 6574 686f 6472  ....classmethodr
+00006780: 2200 0000 7290 0000 0072 c500 0000 7212  "...r....r....r.
+00006790: 0000 0072 cb00 0000 72c7 0000 0072 c600  ...r....r....r..
+000067a0: 0000 7296 0000 0072 8c00 0000 7277 0000  ..r....r....rw..
+000067b0: 0072 2800 0000 72f6 0000 0072 1100 0000  .r(...r....r....
+000067c0: 72f8 0000 0072 fc00 0000 7203 0100 0072  r....r....r....r
+000067d0: 0401 0000 7200 0100 0072 0e00 0000 720a  ....r....r....r.
+000067e0: 0100 0072 9800 0000 7215 0100 0072 2201  ...r....r....r".
+000067f0: 0000 7227 0100 0072 2e01 0000 da0d 5f5f  ..r'...r......__
+00006800: 636c 6173 7363 656c 6c5f 5f72 5300 0000  classcell__rS...
+00006810: 7253 0000 0072 7900 0000 7257 0000 0072  rS...ry...rW...r
+00006820: 4100 0000 4c00 0000 73d2 0100 000a 000c  A...L...s.......
+00006830: 010c 010c 010c 010c 0102 0502 0102 0102  ................
+00006840: 0102 0102 0102 0102 0102 0106 f502 0202  ................
+00006850: fe06 0302 fd06 0402 fc06 0502 fb0a 0602  ................
+00006860: fa0a 0702 f90a 0802 f80a 0902 f706 0a02  ................
+00006870: f602 0b02 f502 0c0e f40e 7102 0602 0104  ..........q.....
+00006880: fd0a 0202 fe02 0302 fd02 040e fc02 2e16  ................
+00006890: 0202 fe02 030a fd02 3404 fd16 0202 fe06  ........4.......
+000068a0: 0302 fd02 0402 fc04 050a fb02 6304 fd0a  ............c...
+000068b0: 0202 fe06 0302 fd02 0402 fc02 050a fb02  ................
+000068c0: 0e1c 0102 0302 0104 0202 fe16 0302 fd06  ................
+000068d0: 040c fc00 7f00 7f02 2220 0102 0324 0102  ........" ...$..
+000068e0: 0324 0102 0302 0402 0104 fc06 0202 fe02  .$..............
+000068f0: 0302 fd02 0402 fc06 050c fb14 3f10 0902  ............?...
+00006900: 1204 0202 fe02 030a fd02 3202 0104 fd0a  ..........2.....
+00006910: 0202 fe08 0302 fd02 040e fc02 1002 0104  ................
+00006920: fd0a 0202 fe08 0302 fd0e 040e fc02 0f02  ................
+00006930: 0102 0104 fc0a 0202 fe0a 0302 fd02 0402  ................
+00006940: fc0e 050a fb02 3002 0102 0104 fc0a 0202  ......0.........
+00006950: fe0a 0302 fd02 0402 fc02 050a fb02 2802  ..............(.
+00006960: 0104 fc04 0202 fe0a 0302 fd02 0402 fc02  ................
+00006970: 050a fb02 2102 010a 0102 ff06 0202 fe0a  ....!...........
+00006980: 030c fd02 0602 0116 0202 fe06 030c fd02  ................
+00006990: 1902 0104 0202 fe16 0302 fd02 040c fc02  ................
+000069a0: 0a02 0602 0102 0104 f902 0202 fe0a 0302  ................
+000069b0: fd06 0402 fc0a 0502 fb0e 0602 fa06 0702  ................
+000069c0: f902 080c f802 6302 0302 0102 0104 fc0e  ......c.........
+000069d0: 0202 fe12 0302 fd16 0402 fc02 0502 fb02  ................
+000069e0: 060c fa02 2e02 0402 0106 fc02 0202 fe0a  ................
+000069f0: 0302 fd0a 0402 fc02 0502 fb02 0614 fa72  ...............r
+00006a00: 4100 0000 294e 7274 0000 00da 0f63 6f6c  A...)Nrt.....col
+00006a10: 6c65 6374 696f 6e73 2e61 6263 72cc 0000  lections.abcr...
+00006a20: 0072 7f00 0000 7202 0000 00da 0a63 6f6e  .r....r......con
+00006a30: 7465 7874 6c69 6272 0300 0000 da0b 6461  textlibr......da
+00006a40: 7461 636c 6173 7365 7372 0400 0000 7205  taclassesr....r.
+00006a50: 0000 0072 0600 0000 da04 656e 756d 7207  ...r......enumr.
+00006a60: 0000 00da 0966 756e 6374 6f6f 6c73 7208  .....functoolsr.
+00006a70: 0000 00da 0769 6e73 7065 6374 7209 0000  .....inspectr...
+00006a80: 00da 0574 7970 6573 720a 0000 00da 0674  ...typesr......t
+00006a90: 7970 696e 6772 0b00 0000 720c 0000 0072  ypingr....r....r
+00006aa0: 0d00 0000 720e 0000 0072 0f00 0000 7210  ....r....r....r.
+00006ab0: 0000 0072 1100 0000 7212 0000 0072 1300  ...r....r....r..
+00006ac0: 0000 7214 0000 0072 1500 0000 5a0d 706b  ..r....r....Z.pk
+00006ad0: 675f 7265 736f 7572 6365 7372 1600 0000  g_resourcesr....
+00006ae0: da07 6163 7469 6f6e 7372 1800 0000 7219  ..actionsr....r.
+00006af0: 0000 0072 1a00 0000 721b 0000 0072 1c00  ...r....r....r..
+00006b00: 0000 721d 0000 0072 1e00 0000 721f 0000  ..r....r....r...
+00006b10: 0072 2000 0000 da03 6172 6772 2100 0000  .r .....argr!...
+00006b20: 7222 0000 0072 2300 0000 7224 0000 0072  r"...r#...r$...r
+00006b30: 2500 0000 da0a 6578 6365 7074 696f 6e73  %.....exceptions
+00006b40: 7226 0000 0072 2700 0000 72bd 0000 0072  r&...r'...r....r
+00006b50: 2800 0000 7229 0000 0072 2a00 0000 722b  (...r)...r*...r+
+00006b60: 0000 00da 0575 7469 6c73 722c 0000 0072  .....utilsr,...r
+00006b70: 2d00 0000 722e 0000 0072 2f00 0000 7230  -...r....r/...r0
+00006b80: 0000 0072 3100 0000 7232 0000 0072 3300  ...r1...r2...r3.
+00006b90: 0000 7234 0000 0072 3500 0000 7236 0000  ..r4...r5...r6..
+00006ba0: 0072 3700 0000 7238 0000 0072 3900 0000  .r7...r8...r9...
+00006bb0: 72c4 0000 0072 3c00 0000 5a11 7479 7069  r....r<...Z.typi
+00006bc0: 6e67 5f65 7874 656e 7369 6f6e 7372 3f00  ng_extensionsr?.
+00006bd0: 0000 7240 0000 0072 4100 0000 7253 0000  ..r@...rA...rS..
+00006be0: 0072 5300 0000 7253 0000 0072 5700 0000  .rS...rS...rW...
+00006bf0: da08 3c6d 6f64 756c 653e 0100 0000 7332  ..<module>....s2
+00006c00: 0000 0008 0008 0108 010c 010c 0114 010c  ................
+00006c10: 010c 010c 010c 0134 010c 0e2c 021c 0b10  .......4...,....
+00006c20: 070c 0114 0140 010a 110e 010c 020a 020c  .....@..........
+00006c30: 0108 0216 03                             .....
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/exceptions.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/exceptions.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 633 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 7902 0000  o.......u..dy...
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 7902 0000  o........I.dy...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 6200 0000 6400  .....@...sb...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 4700  m.Z.m.Z.m.Z...G.
 00000050: 6403 6404 8400 6404 6506 8303 5a07 4700  d.d...d.e...Z.G.
 00000060: 6405 6406 8400 6406 6501 8303 5a08 0907  d.d...d.e...Z...
 00000070: 640c 6408 6505 6503 1900 6409 6504 6506  d.d.e.e...d.e.e.
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/namespace.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/namespace.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 304 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 3001 0000  o.......u..d0...
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 3001 0000  o........I.d0...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 3000 0000 6400  .....@...s0...d.
 00000030: 6401 6c00 6d01 5a02 0100 6400 6402 6c03  d.l.m.Z...d.d.l.
 00000040: 6d04 5a04 6d05 5a05 0100 4700 6403 6404  m.Z.m.Z...G.d.d.
 00000050: 8400 6404 6502 8303 5a01 6405 5300 2906  ..d.e...Z.d.S.).
 00000060: e900 0000 0029 01da 094e 616d 6573 7061  .....)...Namespa
 00000070: 6365 2902 da03 416e 79da 0444 6963 7463  ce)...Any..Dictc
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/types.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/types.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 1300 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 1405 0000  o.......u..d....
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 1405 0000  o........I.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0073 e600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6400 6403 6c03 6d04 5a04 6d05 5a05  ..d.d.l.m.Z.m.Z.
 00000050: 6d06 5a06 6d07 5a07 6d08 5a08 6d09 5a09  m.Z.m.Z.m.Z.m.Z.
 00000060: 0100 6500 6a0a 6404 6b05 7226 6400 6405  ..e.j.d.k.r&d.d.
 00000070: 6c03 6d0b 5a0b 0100 6e06 6400 6405 6c0c  l.m.Z...n.d.d.l.
```

### Comparing `yapx-0.2.0/src/yapx/__pycache__/utils.cpython-310.pyc` & `yapx-0.2.1/src/yapx/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 20 04:17:57 2023 UTC, .py size: 4214 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 75b5 b864 7610 0000  o.......u..dv...
+00000000: 6f0d 0d0a 0000 0000 0b49 bf64 7310 0000  o........I.ds...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 2803 0000 5500  .....@...s(...U.
 00000030: 6400 6401 6c00 5a00 6400 6402 6c01 6d02  d.d.l.Z.d.d.l.m.
 00000040: 5a02 0100 6400 6403 6c03 6d04 5a04 0100  Z...d.d.l.m.Z...
 00000050: 6400 6404 6c05 6d06 5a06 0100 6400 6405  d.d.l.m.Z...d.d.
 00000060: 6c07 6d08 5a08 0100 6400 6406 6c09 6d0a  l.m.Z...d.d.l.m.
 00000070: 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d 6d0e  Z.m.Z.m.Z.m.Z.m.
@@ -242,27 +242,27 @@
 00000f10: 6f72 7256 0000 005a 0870 7964 616e 7469  orrV...Z.pydanti
 00000f20: 6372 2400 0000 7225 0000 005a 1070 7964  cr$...r%...Z.pyd
 00000f30: 616e 7469 635f 7665 7273 696f 6eda 0369  antic_version..i
 00000f40: 6e74 da05 7370 6c69 7472 2700 0000 7229  nt..splitr'...r)
 00000f50: 0000 0072 2a00 0000 5a14 7079 6461 6e74  ...r*...Z.pydant
 00000f60: 6963 2e64 6174 6163 6c61 7373 6573 722b  ic.dataclassesr+
 00000f70: 0000 0072 1300 0000 722f 0000 00da 0945  ...r....r/.....E
-00000f80: 7863 6570 7469 6f6e 5a0f 7472 6f67 6f6e  xceptionZ.trogon
-00000f90: 2e61 7267 7061 7273 6572 3300 0000 7234  .argparser3...r4
-00000fa0: 0000 005a 0d72 6963 685f 6172 6770 6172  ...Z.rich_argpar
-00000fb0: 7365 7235 0000 0072 3600 0000 da08 6172  ser5...r6.....ar
-00000fc0: 6770 6172 7365 da0c 7665 7273 696f 6e5f  gparse..version_
-00000fd0: 696e 666f 7239 0000 00da 1174 7970 696e  infor9.....typin
-00000fe0: 675f 6578 7465 6e73 696f 6e73 7214 0000  g_extensionsr...
-00000ff0: 0072 4000 0000 7242 0000 0072 4400 0000  .r@...rB...rD...
-00001000: 7245 0000 0072 4900 0000 7219 0000 0072  rE...rI...r....r
-00001010: 1a00 0000 7221 0000 0072 2100 0000 7221  ....r!...r!...r!
-00001020: 0000 0072 2200 0000 da08 3c6d 6f64 756c  ...r".....<modul
-00001030: 653e 0100 0000 737e 0000 000a 000c 010c  e>....s~........
-00001040: 010c 010c 0120 0114 030c 050c 0108 020c  ..... ..........
-00001050: 0e0c 020c 010c 010c 0102 0310 0108 020c  ................
-00001060: 0108 0214 0302 fb02 080c 010c 011c 020c  ................
-00001070: 0108 020c 010c 011c 040c 040c 0108 020c  ................
-00001080: 0108 0208 0314 0302 f802 0c10 0108 020e  ................
-00001090: 0108 020c 0302 fb02 090c 0108 020e 0110  ................
-000010a0: 0102 ff0c 030e 010c 021a 0306 0418 0106  ................
-000010b0: 0618 011c 061c 0622 12                   .......".
+00000f80: 7863 6570 7469 6f6e 5a0c 6172 6770 6172  xceptionZ.argpar
+00000f90: 7365 5f74 7569 7233 0000 0072 3400 0000  se_tuir3...r4...
+00000fa0: 5a0d 7269 6368 5f61 7267 7061 7273 6572  Z.rich_argparser
+00000fb0: 3500 0000 7236 0000 00da 0861 7267 7061  5...r6.....argpa
+00000fc0: 7273 65da 0c76 6572 7369 6f6e 5f69 6e66  rse..version_inf
+00000fd0: 6f72 3900 0000 da11 7479 7069 6e67 5f65  or9.....typing_e
+00000fe0: 7874 656e 7369 6f6e 7372 1400 0000 7240  xtensionsr....r@
+00000ff0: 0000 0072 4200 0000 7244 0000 0072 4500  ...rB...rD...rE.
+00001000: 0000 7249 0000 0072 1900 0000 721a 0000  ..rI...r....r...
+00001010: 0072 2100 0000 7221 0000 0072 2100 0000  .r!...r!...r!...
+00001020: 7222 0000 00da 083c 6d6f 6475 6c65 3e01  r".....<module>.
+00001030: 0000 0073 7e00 0000 0a00 0c01 0c01 0c01  ...s~...........
+00001040: 0c01 2001 1403 0c05 0c01 0802 0c0e 0c02  .. .............
+00001050: 0c01 0c01 0c01 0203 1001 0802 0c01 0802  ................
+00001060: 1403 02fb 0208 0c01 0c01 1c02 0c01 0802  ................
+00001070: 0c01 0c01 1c04 0c04 0c01 0802 0c01 0802  ................
+00001080: 0803 1403 02f8 020c 1001 0802 0e01 0802  ................
+00001090: 0c03 02fb 0209 0c01 0802 0e01 1001 02ff  ................
+000010a0: 0c03 0e01 0c02 1a03 0604 1801 0606 1801  ................
+000010b0: 1c06 1c06 2212                           ....".
```

### Comparing `yapx-0.2.0/src/yapx/actions.py` & `yapx-0.2.1/src/yapx/actions.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,58 +20,56 @@
         default=None,
         type=None,  # pylint: disable=redefined-builtin
         choices=None,
         required=False,
         help=None,  # pylint: disable=redefined-builtin
         metavar=None,
     ):
-        self._base_case_is_negative: bool = False
-        self._negative_option_strings: List[str] = []
-
-        if option_strings:
-            self._base_case_is_negative = any(
-                x.startswith(self.NEGATION_PREFIX) for x in option_strings
-            )
-
-            if self._base_case_is_negative and default is not None:
-                default = not default
+        self._negation_option_strings: List[str] = []
 
         _option_strings = []
         for option_string in option_strings:
-            if "/" in option_string:
+            if not option_string.startswith("--"):
+                _option_strings.append(option_string)
+            elif "/" in option_string:
                 opt_str, opt_str_neg = map(
                     str.strip,
                     option_string.split("/", maxsplit=1),
                 )
 
                 _option_strings.extend([opt_str, opt_str_neg])
-                self._negative_option_strings.append(opt_str_neg)
-            elif not option_string.startswith("--"):
-                _option_strings.append(option_string)
+
+                self._negation_option_strings.append(opt_str_neg)
             elif not option_string.startswith(self.NEGATION_PREFIX):
+                opt_str_neg = self.NEGATION_PREFIX + option_string[2:]
                 _option_strings.extend(
                     [
                         option_string,
-                        self.NEGATION_PREFIX + option_string[2:],
-                    ],
-                )
-            elif default is False:
-                _option_strings.extend(
-                    [
-                        "--" + option_string[len(self.NEGATION_PREFIX) :],
-                        option_string,
-                    ],
-                )
-            else:  # elif default is None or default:
-                _option_strings.extend(
-                    [
-                        option_string,
-                        "--" + option_string[len(self.NEGATION_PREFIX) :],
+                        opt_str_neg,
                     ],
                 )
+                self._negation_option_strings.append(opt_str_neg)
+            else:  # if option_string.startswith(self.NEGATION_PREFIX):
+                opt_str_neg = "--" + option_string[len(self.NEGATION_PREFIX) :]
+                if default is False:
+                    _option_strings.extend(
+                        [
+                            opt_str_neg,
+                            option_string,
+                        ],
+                    )
+                else:  # elif default is None or default:
+                    _option_strings.extend(
+                        [
+                            option_string,
+                            opt_str_neg,
+                        ],
+                    )
+
+                self._negation_option_strings.append(opt_str_neg)
 
         super().__init__(
             option_strings=_option_strings,
             dest=dest,
             nargs=0,
             default=default,
             type=type,
@@ -79,20 +77,15 @@
             required=required,
             help=help,
             metavar=metavar,
         )
 
     def __call__(self, parser, namespace, values, option_string=None):
         if option_string:
-            value: bool = (
-                not option_string.startswith(self.NEGATION_PREFIX)
-                and option_string not in self._negative_option_strings
-            )
-            if self._base_case_is_negative and value is not None:
-                value = not value
+            value: bool = option_string not in self._negation_option_strings
         else:
             dest_type: Type[Any] = parser._dest_type.get(self.dest, bool)
             value = dest_type(values)
 
         setattr(
             namespace,
             self.dest,
```

### Comparing `yapx-0.2.0/src/yapx/arg.py` & `yapx-0.2.1/src/yapx/arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/src/yapx/argument_parser.py` & `yapx-0.2.1/src/yapx/argument_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,14 +99,16 @@
             prog=prog,
             description=None if _is_subparser else description,
             add_help=False,
             formatter_class=formatter_class,
             **kwargs,
         )
 
+        self._subparsers_action: Optional[argparse._SubParsersAction] = None
+
         # self._positionals.title = "commands"
         self._optionals.title = "helpful parameters"
 
         if help_flags is None:
             help_flags = ["-h", "--help"]
 
         if help_flags:
@@ -174,14 +176,15 @@
                 tui_flags = ["--tui"]
 
             if tui_flags and is_tui_available:
                 if isinstance(tui_flags, str):
                     tui_flags = [tui_flags]
 
                 if len(tui_flags) == 1 and not tui_flags[0].startswith("-"):
+                    self._get_or_add_subparsers()
                     add_tui_command(
                         parser=self,
                         option_strings=tui_flags[0],
                         help="Show Textual User Interface (TUI).",
                     )
                 else:
                     add_tui_argument(
@@ -227,19 +230,20 @@
 
         # don't include usage in help text.
         usage = self.usage
         self.usage = argparse.SUPPRESS
 
         super().print_help(file)
 
-        if include_commands:
-            subparsers: Optional[argparse._SubParsersAction] = self._get_subparsers()
-            if subparsers:
-                for _choice, subparser in subparsers.choices.items():
-                    subparser.print_help(file, include_commands=include_commands)
+        if include_commands and self._subparsers:
+            if self._subparsers_action is None:
+                self._subparsers_action = self._find_subparsers_action()
+
+            for _choice, subparser in self._subparsers_action.choices.items():
+                subparser.print_help(file, include_commands=include_commands)
 
         self.usage = usage
 
     def add_arguments(
         self,
         args_model: Union[Callable[..., Any], Type[Dataclass]],
     ) -> None:
@@ -763,39 +767,40 @@
             and type_container_subtype_origin
             and not is_pydantic_available
         ):
             raise_unsupported_type_error(type_container_subtype_origin)
 
         return type_container_subtype
 
-    def _get_subparsers(self) -> Optional[argparse._SubParsersAction]:
+    def _find_subparsers_action(self) -> Optional[argparse._SubParsersAction]:
         for a in self._actions:
             if isinstance(
                 a,
                 argparse._SubParsersAction,  # pylint: disable=protected-access
             ):
                 return a
         return None
 
     def _get_or_add_subparsers(self) -> argparse._SubParsersAction:
-        subparsers = self._get_subparsers()
-
-        if not subparsers:
-            subparsers = self.add_subparsers(
-                title="commands",
-                metavar="<COMMAND>",
-                dest=self.CMD_ATTR_NAME,
-                parser_class=lambda **k: type(self)(
-                    **k,
-                    _is_subparser=True,
-                    formatter_class=self.formatter_class,
-                ),
-            )
+        if self._subparsers_action is None:
+            if self._subparsers:
+                self._subparsers_action = self._find_subparsers_action()
+            else:
+                self._subparsers_action = self.add_subparsers(
+                    title="commands",
+                    metavar="<COMMAND>",
+                    dest=self.CMD_ATTR_NAME,
+                    parser_class=lambda **k: type(self)(
+                        **k,
+                        _is_subparser=True,
+                        formatter_class=self.formatter_class,
+                    ),
+                )
 
-        return subparsers
+        return self._subparsers_action
 
     def _post_parse_args(  # type: ignore[override]
         self,
         namespace: argparse.Namespace,
     ) -> Namespace:
         func_mx_arg_groups: Dict[
             str,
```

### Comparing `yapx-0.2.0/src/yapx/exceptions.py` & `yapx-0.2.1/src/yapx/exceptions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/src/yapx/types.py` & `yapx-0.2.1/src/yapx/types.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/src/yapx/utils.py` & `yapx-0.2.1/src/yapx/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         ...
 
     class ValidationError(Exception):
         ...
 
 
 try:
-    from trogon.argparse import add_tui_argument, add_tui_command
+    from argparse_tui import add_tui_argument, add_tui_command
 
     is_tui_available = True
 except ModuleNotFoundError:
 
     def add_tui_argument():
         ...
```

### Comparing `yapx-0.2.0/src/yapx.egg-info/PKG-INFO` & `yapx-0.2.1/src/yapx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 Metadata-Version: 2.1
 Name: yapx
-Version: 0.2.0
+Version: 0.2.1
 Summary: Build awesome Python CLIs with ease.
 Author-email: Donald Mellenbruch <hello@f2dv.com>
 License: Copyright 2023 Donald Mellenbruch
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
         
         THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
         
 Project-URL: Homepage, https://www.f2dv.com/code/r/yapx/i
 Project-URL: Repository, https://www.github.com/fresh2dev/yapx
-Project-URL: Funding, https://www.f2dv.com/funding
+Project-URL: Funding, https://www.f2dv.com/fund
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: tests
 Provides-Extra: pydantic
 Provides-Extra: shtab
 Provides-Extra: rich
+Provides-Extra: tui
 Provides-Extra: extras
 License-File: LICENSE
 
 # yapx
 
 > Build awesome Python CLIs with ease.
 
 | Links         |                                              |
 |---------------|----------------------------------------------|
 | Code Repo     | https://www.github.com/fresh2dev/yapx        |
 | Mirror Repo   | https://www.f2dv.com/code/r/yapx             |
 | Documentation | https://www.f2dv.com/code/r/yapx/i           |
 | Changelog     | https://www.f2dv.com/code/r/yapx/i/changelog |
 | License       | https://www.f2dv.com/code/r/yapx/i/license   |
-| Funding       | https://www.f2dv.com/funding                 |
+| Funding       | https://www.f2dv.com/fund                    |
 
 [![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/releases)
 [![License](https://img.shields.io/github/license/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.f2dv.com/code/r/yapx/i/license)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/yapx?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/yapx/pulls)
 [![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/yapx?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/yapx&Date)
@@ -77,16 +78,16 @@
 ```
 
 Extras are available to unlock additional functionality:
 
 - `yapx[pydantic]`: enables support for additional types
 - `yapx[shtab]`: enables shell-completion
 - `yapx[rich]`: enables prettier help and error messages
+- `yapx[tui]`: enables experimental TUI support
 - `yapx[extras]`: enables each of the above
-- `trogon-yapx`: enables experimental TUI support
 
 ## Use
 
 See notebooks of examples here:
 
 https://www.f2dv.com/code/r/yapx/i/page/overview
```

### Comparing `yapx-0.2.0/src/yapx.egg-info/SOURCES.txt` & `yapx-0.2.1/src/yapx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/src/yapx.egg-info/requires.txt` & `yapx-0.2.1/src/yapx.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -24,29 +24,33 @@
 mkdocs-autorefs==0.*
 mkdocs-include-dir-to-nav==1.*
 
 [extras]
 pydantic<3,>=1.10.3
 shtab==1.6.2
 rich-argparse==1.*
+argparse-tui<1,>=0.1.2
 
 [pydantic]
 pydantic<3,>=1.10.3
 
 [rich]
 rich-argparse==1.*
 
 [shtab]
-shtab==1.6.2
+shtab==1.6.*
 
 [tests]
 pytest==7.*
 pytest-cov==4.*
 pytest-html==3.*
 pytest-sugar==0.*
 pytest-custom-exit-code==0.3.*
 pylint==2.*
 pylint-pytest==1.*
 packaging==23.*
 pydantic<3,>=1.10.3
-shtab==1.6.2
+shtab==1.6.*
 rich-argparse==1.*
+
+[tui]
+argparse-tui<1,>=0.1.2
```

### Comparing `yapx-0.2.0/tests/test_actions.py` & `yapx-0.2.1/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/tests/test_add_arguments.py` & `yapx-0.2.1/tests/test_add_arguments.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/tests/test_add_arguments_future.py` & `yapx-0.2.1/tests/test_add_arguments_future.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/tests/test_add_command.py` & `yapx-0.2.1/tests/test_add_command.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/tests/test_arg.py` & `yapx-0.2.1/tests/test_arg.py`

 * *Files identical despite different names*

### Comparing `yapx-0.2.0/tests/test_run.py` & `yapx-0.2.1/tests/test_run.py`

 * *Files 1% similar despite different names*

```diff
@@ -705,25 +705,27 @@
         verbose: Annotated[int, yapx.arg(default=0, nargs=0, flags="-v")],
         live: bool,
         dye: Annotated[bool, yapx.arg(pos=True)],
         start: Annotated[bool, yapx.arg(flags=["--init/--no-init", "-x/-X"])] = False,
         feet: Annotated[str, yapx.arg(nargs=0, flags=["--dev", "--prod"])] = "nada",
         stop: bool = True,
         no_fear: bool = True,
+        no_doubt: bool = False,
         fly: Optional[bool] = None,
         dowat: Optional[List[bool]] = None,
     ):
         assert dye is True
         assert verbose == 5
         assert live is True
         assert stop is False
         assert start is True
         assert feet == "prod"
         assert stop is False
         assert no_fear is False
+        assert no_doubt is False
         assert fly is False
         assert dowat == [True, False]
 
     cli_args: List[str] = [
         "true",
         "--live",
         "--stop",
```

### Comparing `yapx-0.2.0/tests/test_utils.py` & `yapx-0.2.1/tests/test_utils.py`

 * *Files identical despite different names*

