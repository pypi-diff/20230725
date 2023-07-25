# Comparing `tmp/bitsrun-3.5.2.tar.gz` & `tmp/bitsrun-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitsrun-3.5.2.tar", last modified: Tue May  9 10:13:24 2023, max compression
+gzip compressed data, was "bitsrun-3.6.0.tar", last modified: Tue Jul 25 09:45:27 2023, max compression
```

## Comparing `bitsrun-3.5.2.tar` & `bitsrun-3.6.0.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0      496 2023-05-09 10:12:57.953702 bitsrun-3.5.2/LICENSE
--rw-r--r--   0        0        0     3445 2023-05-09 10:12:57.953702 bitsrun-3.5.2/README.md
--rw-r--r--   0        0        0        0 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/__init__.py
--rw-r--r--   0        0        0     4811 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/cli.py
--rw-r--r--   0        0        0     2332 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/config.py
--rw-r--r--   0        0        0      891 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/models.py
--rw-r--r--   0        0        0     4921 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/user.py
--rw-r--r--   0        0        0     4193 2023-05-09 10:12:57.953702 bitsrun-3.5.2/bitsrun/utils.py
--rw-r--r--   0        0        0     1739 2023-05-09 10:12:57.953702 bitsrun-3.5.2/pyproject.toml
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 bitsrun-3.5.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:27.762092 bitsrun-3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 09:45:07.000000 bitsrun-3.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-25 09:45:27.758092 bitsrun-3.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-25 09:45:07.000000 bitsrun-3.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-25 09:45:07.000000 bitsrun-3.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 09:45:27.762092 bitsrun-3.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:27.754092 bitsrun-3.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:27.758092 bitsrun-3.6.0/src/bitsrun/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4921 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-07-25 09:45:07.000000 bitsrun-3.6.0/src/bitsrun/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 09:45:27.758092 bitsrun-3.6.0/src/bitsrun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 09:45:27.000000 bitsrun-3.6.0/src/bitsrun.egg-info/top_level.txt
```

### Comparing `bitsrun-3.5.2/README.md` & `bitsrun-3.6.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # bitsrun
 
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://github.com/BITNP/bitsrun/actions/workflows/ci.yml/badge.svg)](https://github.com/BITNP/bitsrun/actions/workflows/ci.yml)
 [![PyPI Publish](https://github.com/BITNP/bitsrun/actions/workflows/python-publish.yml/badge.svg)](https://github.com/BITNP/bitsrun/actions/workflows/python-publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/bitsrun)](https://pypi.org/project/bitsrun/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bitsrun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/bitsrun)
 
 _A headless login / logout script for 10.0.0.55 at BIT._
@@ -98,37 +97,34 @@
 
 ![raycast screenshot](https://user-images.githubusercontent.com/32114380/213919582-eff6d58f-1bd2-47b2-a5da-46dc6e2eaffa.png)
 
 Import the two Raycast scripts from [`./scripts`](./scripts/) and setup your config file in `~/.config/bit-user.json`. The script uses `/usr/bin/python3` by default, so you either need to install `bitsrun` with this Python interpreter or setup your own Python interpreter path in the script.
 
 ## Developing
 
-Install and run:
+Create virtual environment and install deps:
 
 ```shell
-# Create virtual env and install deps
-pdm install
-
-# Enter virtual env
-eval $(pdm venv activate)
-
-# Install pre-commit hooks
-pre-commit install
+python -m venv venv
+source venv/bin/activate
+pip install -r requirements.txt
+pip install -e .
 ```
 
-Build:
+Running CLI entry:
 
 ```shell
-pdm build
+python src/bitsrun/cli.py
 ```
 
-Publish:
+Build:
 
 ```shell
-pdm publish
+pip install setuptools build
+python -m build
 ```
 
 ## Credits
 
 - [Aloxaf/10_0_0_55_login](https://github.com/Aloxaf/10_0_0_55_login)
 
 ## License
```

### Comparing `bitsrun-3.5.2/bitsrun/cli.py` & `bitsrun-3.6.0/src/bitsrun/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # https://stackoverflow.com/questions/40182157/shared-options-and-flags-between-commands
 _options = [
     click.option("-u", "--username", help="Your username.", required=False),
     click.option("-p", "--password", help="Your password.", required=False),
     click.option("-v", "--verbose", is_flag=True, help="Verbosely echo API response."),
 ]
 
-
 # Replace the default implementation
 warnings.showwarning = (
     lambda message, category, filename, lineno, file=None, line=None: click.echo(
         f"{click.style('warning:', fg='yellow')} {message}", err=True
     )
 )
```

### Comparing `bitsrun-3.5.2/bitsrun/config.py` & `bitsrun-3.6.0/src/bitsrun/config.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.2/bitsrun/models.py` & `bitsrun-3.6.0/src/bitsrun/models.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.2/bitsrun/user.py` & `bitsrun-3.6.0/src/bitsrun/user.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.2/bitsrun/utils.py` & `bitsrun-3.6.0/src/bitsrun/utils.py`

 * *Files identical despite different names*

### Comparing `bitsrun-3.5.2/pyproject.toml` & `bitsrun-3.6.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,23 @@
 [project]
 name = "bitsrun"
-version = "3.5.2"
+version = "3.6.0"
 description = "A headless login / logout script for 10.0.0.55"
-authors = [
-    { name = "spencerwooo", email = "spencer.woo@outlook.com" },
-]
+authors = [{ name = "spencerwooo", email = "spencer.woo@outlook.com" }]
 dependencies = [
     "httpx>=0.24.0",
     "rich>=13.3.5",
     "humanize>=4.5.0",
     "click>=8.1.3",
     "platformdirs>=2.6.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
-keywords = [
-    "bit",
-    "srun",
-    "srun-login",
-    "srun-client",
-    "beijing-institute-of-technology",
-]
+license = { text = "WTFPL" }
+keywords = ["bit", "srun", "srun-login", "srun-client", "beijing-institute-of-technology"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Education",
     "Intended Audience :: End Users/Desktop",
     "Intended Audience :: Information Technology",
@@ -34,52 +27,27 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Education",
     "Topic :: Internet",
 ]
 
-[project.license]
-text = "WTFPL"
-
 [project.urls]
 homepage = "https://github.com/BITNP/bitsrun"
 
 [project.scripts]
 bitsrun = "bitsrun.cli:cli"
 
-[tool.pdm.dev-dependencies]
-dev = [
-    "black>=23.3.0",
-    "ruff>=0.0.265",
-    "mypy>=1.2.0",
-    "pre-commit>=3.3.1",
-]
-
-[tool.pdm.build]
-includes = []
-
-[tool.pdm.scripts]
-lint = "pre-commit run --all-files"
-type-check = "mypy bitsrun"
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
 [tool.ruff]
 line-length = 88
-select = [
-    "E",
-    "F",
-    "I",
-    "N",
-    "B",
-    "SIM",
-]
+select = ["E", "F", "I", "N", "B", "SIM"]
 
 [tool.mypy]
 disallow_any_unimported = true
 no_implicit_optional = true
 check_untyped_defs = true
-
-[build-system]
-requires = [
-    "pdm-pep517>=1.0.0",
-]
-build-backend = "pdm.pep517.api"
+# disallow_untyped_defs = true
+# warn_return_any = true
```

### Comparing `bitsrun-3.5.2/PKG-INFO` & `bitsrun-3.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 Metadata-Version: 2.1
 Name: bitsrun
-Version: 3.5.2
+Version: 3.6.0
 Summary: A headless login / logout script for 10.0.0.55
+Author-email: spencerwooo <spencer.woo@outlook.com>
 License: WTFPL
+Project-URL: homepage, https://github.com/BITNP/bitsrun
 Keywords: bit,srun,srun-login,srun-client,beijing-institute-of-technology
-Author-email: spencerwooo <spencer.woo@outlook.com>
-Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Information Technology
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Internet
-Project-URL: homepage, https://github.com/BITNP/bitsrun
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # bitsrun
 
-[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v1.json)](https://github.com/charliermarsh/ruff)
-[![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
+[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/charliermarsh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 [![Pre-commit](https://github.com/BITNP/bitsrun/actions/workflows/ci.yml/badge.svg)](https://github.com/BITNP/bitsrun/actions/workflows/ci.yml)
 [![PyPI Publish](https://github.com/BITNP/bitsrun/actions/workflows/python-publish.yml/badge.svg)](https://github.com/BITNP/bitsrun/actions/workflows/python-publish.yml)
 [![PyPI](https://img.shields.io/pypi/v/bitsrun)](https://pypi.org/project/bitsrun/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/bitsrun)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/bitsrun)
 
 _A headless login / logout script for 10.0.0.55 at BIT._
@@ -123,40 +123,36 @@
 
 ![raycast screenshot](https://user-images.githubusercontent.com/32114380/213919582-eff6d58f-1bd2-47b2-a5da-46dc6e2eaffa.png)
 
 Import the two Raycast scripts from [`./scripts`](./scripts/) and setup your config file in `~/.config/bit-user.json`. The script uses `/usr/bin/python3` by default, so you either need to install `bitsrun` with this Python interpreter or setup your own Python interpreter path in the script.
 
 ## Developing
 
-Install and run:
+Create virtual environment and install deps:
 
 ```shell
-# Create virtual env and install deps
-pdm install
-
-# Enter virtual env
-eval $(pdm venv activate)
-
-# Install pre-commit hooks
-pre-commit install
+python -m venv venv
+source venv/bin/activate
+pip install -r requirements.txt
+pip install -e .
 ```
 
-Build:
+Running CLI entry:
 
 ```shell
-pdm build
+python src/bitsrun/cli.py
 ```
 
-Publish:
+Build:
 
 ```shell
-pdm publish
+pip install setuptools build
+python -m build
 ```
 
 ## Credits
 
 - [Aloxaf/10_0_0_55_login](https://github.com/Aloxaf/10_0_0_55_login)
 
 ## License
 
 [WTFPL License](LICENSE)
-
```

