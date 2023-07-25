# Comparing `tmp/pyslowloris-2.0.1.tar.gz` & `tmp/pyslowloris-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslowloris-2.0.1.tar", last modified: Mon Aug 31 15:17:56 2020, max compression
+gzip compressed data, was "pyslowloris-2.0.2.tar", max compression
```

## Comparing `pyslowloris-2.0.1.tar` & `pyslowloris-2.0.2.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1067 2020-08-31 14:44:00.610400 pyslowloris-2.0.1/LICENSE
--rw-r--r--   0        0        0     3821 2020-08-31 15:08:20.023481 pyslowloris-2.0.1/README.md
--rw-r--r--   0        0        0     1638 2020-08-31 15:17:51.955507 pyslowloris-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     1192 2020-08-31 15:08:20.024259 pyslowloris-2.0.1/pyslowloris/__init__.py
--rw-r--r--   0        0        0     3182 2020-08-31 15:08:20.024387 pyslowloris-2.0.1/pyslowloris/__main__.py
--rw-r--r--   0        0        0     3333 2020-08-31 15:08:20.024469 pyslowloris-2.0.1/pyslowloris/attack.py
--rw-r--r--   0        0        0     3761 2020-08-31 15:08:20.024566 pyslowloris-2.0.1/pyslowloris/connection.py
--rw-r--r--   0        0        0     1420 2020-08-31 15:08:20.024653 pyslowloris-2.0.1/pyslowloris/exceptions.py
--rw-r--r--   0        0        0      506 2020-08-31 15:08:20.024728 pyslowloris-2.0.1/pyslowloris/logger.py
--rw-r--r--   0        0        0     3234 2020-08-31 15:08:20.024830 pyslowloris-2.0.1/pyslowloris/uri_info.py
--rw-r--r--   0        0        0     1515 2020-08-31 15:08:20.026049 pyslowloris-2.0.1/pyslowloris/utils.py
--rw-r--r--   0        0        0     4911 2020-08-31 15:17:56.988354 pyslowloris-2.0.1/setup.py
--rw-r--r--   0        0        0     5055 2020-08-31 15:17:56.988736 pyslowloris-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-07-25 12:47:01.300708 pyslowloris-2.0.2/LICENSE
+-rw-r--r--   0        0        0     3821 2023-07-25 12:47:01.300708 pyslowloris-2.0.2/README.md
+-rw-r--r--   0        0        0     1726 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1192 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/__init__.py
+-rw-r--r--   0        0        0     3182 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/__main__.py
+-rw-r--r--   0        0        0     3333 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/attack.py
+-rw-r--r--   0        0        0     3761 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/connection.py
+-rw-r--r--   0        0        0     1420 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/exceptions.py
+-rw-r--r--   0        0        0      506 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/logger.py
+-rw-r--r--   0        0        0     3234 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/uri_info.py
+-rw-r--r--   0        0        0     1515 2023-07-25 12:47:01.304708 pyslowloris-2.0.2/pyslowloris/utils.py
+-rw-r--r--   0        0        0     5157 1970-01-01 00:00:00.000000 pyslowloris-2.0.2/PKG-INFO
```

### Comparing `pyslowloris-2.0.1/LICENSE` & `pyslowloris-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/README.md` & `pyslowloris-2.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # PySlowLoris
 [![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/SlowLoris-dev/Lobby)
 [![License](https://img.shields.io/badge/license-MIT%20license-orange.svg)](https://github.com/maxkrivich/SlowLoris/blob/master/LICENSE)
 [![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/maxkrivich/SlowLoris)
 [![Build Status](https://travis-ci.org/maxkrivich/SlowLoris.svg?branch=master)](https://travis-ci.org/maxkrivich/SlowLoris)
-[![PyPI version](https://badge.fury.io/py/PySlowLoris.svg)](https://badge.fury.io/py/PySlowLoris)
+[![PyPI version](https://badge.fury.io/py/pyslowloris.svg)](https://badge.fury.io/py/pyslowloris)
 
 PySlowLoris is a tool for testing if your web server is vulnerable to slow-requests kind of attacks. The module is based on python-trio for Asynchronous I/O and poetry for dependency management. The idea behind this approach to create as many connections with a server as possible and keep them alive and send trash headers through the connection. Please DO NOT use this in the real attacks on the servers.
 
 More information about the attack you can find [here].
 
 ### Installation
 
 #### PyPi
 
 For installation through the PyPI:
 
 ```sh
-$ pip install pyslowloris==2.0.0
+$ pip install pyslowloris==2.0.1
 ```
 This method is prefered for installation of the most recent stable release.
 
 
 #### Source-code
 
 For installation through the source-code for local development:
```

### Comparing `pyslowloris-2.0.1/pyproject.toml` & `pyslowloris-2.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "pyslowloris"
-version = "2.0.1"
+version = "2.0.2"
 description = "Asynchronous Python implementation of SlowLoris DoS attack"
 authors = ["Maxim Krivich <maxkrivich@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxkrivich/SlowLoris"
 repository = "https://github.com/maxkrivich/SlowLoris"
 packages = [
     { include = "pyslowloris", from="." }
 ]
 
-
 keywords = [
     "SlowLoris", "dos", "slowloris", "apache", "dos-attacks", "denial-of-service", "http",
     "exploit", "dos-tool", "hacker-scripts", "hacking-tool", "hacking", "vulnerability", "slow-requests",
     "cybersecurity", "cyber-security", "information-security", "security"
 ]
 
 classifiers = [
@@ -37,14 +36,17 @@
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.0.1"
 flake8 = "^3.8.3"
 pytest-trio = "^0.6.0"
 isort = "^5.4.2"
 
+[tool.poetry.group.dev.dependencies]
+pytest-github-actions-annotate-failures = "^0.2.0"
+
 [tool.pytest.ini_options]
 minversion = "6.0.1"
 addopts = "-ra -q -v"
 trio_mode = "true"
 testpaths = [
     "tests"
 ]
```

### Comparing `pyslowloris-2.0.1/pyslowloris/__init__.py` & `pyslowloris-2.0.2/pyslowloris/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/__main__.py` & `pyslowloris-2.0.2/pyslowloris/__main__.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/attack.py` & `pyslowloris-2.0.2/pyslowloris/attack.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/connection.py` & `pyslowloris-2.0.2/pyslowloris/connection.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/exceptions.py` & `pyslowloris-2.0.2/pyslowloris/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/uri_info.py` & `pyslowloris-2.0.2/pyslowloris/uri_info.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/pyslowloris/utils.py` & `pyslowloris-2.0.2/pyslowloris/utils.py`

 * *Files identical despite different names*

### Comparing `pyslowloris-2.0.1/setup.py` & `pyslowloris-2.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,41 +1,159 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyslowloris
+Version: 2.0.2
+Summary: Asynchronous Python implementation of SlowLoris DoS attack
+Home-page: https://github.com/maxkrivich/SlowLoris
+License: MIT
+Keywords: SlowLoris,dos,slowloris,apache,dos-attacks,denial-of-service,http,exploit,dos-tool,hacker-scripts,hacking-tool,hacking,vulnerability,slow-requests,cybersecurity,cyber-security,information-security,security
+Author: Maxim Krivich
+Author-email: maxkrivich@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: System Administrators
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fake-useragent (>=0.1.11,<0.2.0)
+Requires-Dist: jk-triologging (>=0.2019.10,<0.2020.0)
+Requires-Dist: sh (>=1.14.0,<2.0.0)
+Requires-Dist: trio (>=0.16.0,<0.17.0)
+Project-URL: Bug Tracker, https://github.com/maxkrivich/SlowLoris/issues
+Project-URL: Repository, https://github.com/maxkrivich/SlowLoris
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': '.'}
+# PySlowLoris
+[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/SlowLoris-dev/Lobby)
+[![License](https://img.shields.io/badge/license-MIT%20license-orange.svg)](https://github.com/maxkrivich/SlowLoris/blob/master/LICENSE)
+[![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/maxkrivich/SlowLoris)
+[![Build Status](https://travis-ci.org/maxkrivich/SlowLoris.svg?branch=master)](https://travis-ci.org/maxkrivich/SlowLoris)
+[![PyPI version](https://badge.fury.io/py/pyslowloris.svg)](https://badge.fury.io/py/pyslowloris)
 
-packages = \
-['pyslowloris']
+PySlowLoris is a tool for testing if your web server is vulnerable to slow-requests kind of attacks. The module is based on python-trio for Asynchronous I/O and poetry for dependency management. The idea behind this approach to create as many connections with a server as possible and keep them alive and send trash headers through the connection. Please DO NOT use this in the real attacks on the servers.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fake-useragent>=0.1.11,<0.2.0',
- 'jk-triologging>=0.2019.10,<0.2020.0',
- 'sh>=1.14.0,<2.0.0',
- 'trio>=0.16.0,<0.17.0']
-
-entry_points = \
-{'console_scripts': ['slowloris = pyslowloris.__main__:main']}
-
-setup_kwargs = {
-    'name': 'pyslowloris',
-    'version': '2.0.1',
-    'description': 'Asynchronous Python implementation of SlowLoris DoS attack',
-    'long_description': '# PySlowLoris\n[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/SlowLoris-dev/Lobby)\n[![License](https://img.shields.io/badge/license-MIT%20license-orange.svg)](https://github.com/maxkrivich/SlowLoris/blob/master/LICENSE)\n[![Python](https://img.shields.io/badge/python-3.8-blue.svg)](https://github.com/maxkrivich/SlowLoris)\n[![Build Status](https://travis-ci.org/maxkrivich/SlowLoris.svg?branch=master)](https://travis-ci.org/maxkrivich/SlowLoris)\n[![PyPI version](https://badge.fury.io/py/PySlowLoris.svg)](https://badge.fury.io/py/PySlowLoris)\n\nPySlowLoris is a tool for testing if your web server is vulnerable to slow-requests kind of attacks. The module is based on python-trio for Asynchronous I/O and poetry for dependency management. The idea behind this approach to create as many connections with a server as possible and keep them alive and send trash headers through the connection. Please DO NOT use this in the real attacks on the servers.\n\nMore information about the attack you can find [here].\n\n### Installation\n\n#### PyPi\n\nFor installation through the PyPI:\n\n```sh\n$ pip install pyslowloris==2.0.0\n```\nThis method is prefered for installation of the most recent stable release.\n\n\n#### Source-code\n\nFor installation through the source-code for local development:\n```sh\n$ git clone https://github.com/[username]/SlowLoris.git\n$ cd SlowLoris\n$ pip install poetry\n$ pyenv install 3.8.3\n$ pyenv local 3.8.3\n$ poetry env use 3.8.3\n```\n\n### Basic Usage\n\nAvailable command list:\n\n```sh\n$ slowloris --help\nusage: slowloris [-h] -u URL [-c CONNECTION_COUNT] [-s]\n\nAsynchronous Python implementation of SlowLoris attack\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -u URL, --url URL     Link to a web server (http://google.com) - str\n  -c CONNECTION_COUNT, --connection-count CONNECTION_COUNT\n                        Count of active connections (default value is 247) - int\n  -s, --silent          Ignore all of the errors [pure attack mode] - bool\n```\n\n### Docker usage\n\n#### Download image from Docker Hub\n\nPull the image from [Docker Hub](https://hub.docker.com/r/maxkrivich/pyslowloris/) and run a container:\n\n```bash\n$ docker pull maxkrivich/pyslowloris\n$ docker run --rm -it maxkrivich/pyslowloris [-h] [-u URL] [-c CONNECTION_COUNT] [-s SILENT]\n```\n\n#### Build image from source-code\n\nAlso you can build image from [Dockerfile](https://github.com/maxkrivich/SlowLoris/blob/master/Dockerfile) and run a container:\n\n```bash\n$ docker build -t pyslowloris .\n$ docker run --rm -it pyslowloris [-h] [-u URL] [-c CONNECTION_COUNT] [-s SILENT]\n```\n\n**Note:** *Don\'t forget about \'sudo\'!*\n\n\n\n### Example of usage\n\n#### How to use module through Python API\nHere is an example of usage\n\n```python\nfrom pyslowloris import HostAddress, SlowLorisAttack\n\nurl = HostAddress.from_url("http://kpi.ua")\nconnections_count = 100\n\nloris = SlowLorisAttack(url, connections_count, silent=True)\nloris.start()\n```\n\n#### How to use module via CLI\n\nThe following command helps to use module from command line\n\n```sh\n$ slowloris -u http://kpi.ua/ -c 100 -s\n```\n###### stop execution: Ctrl + C\n\n\n\n### Testing\n\n#### Testing with real apache server\n\n```bash\n$ docker-compose up web_server -d\n$ .....\n```\n\n#### Module-tests\n```bash\n$ make pytest\n```\n\n### Bugs, issues and contributing\n\nIf you find [bugs] or have [suggestions] about improving the module, don\'t hesitate to contact me.\n\n### License\n\nThis project is licensed under the MIT License - see the [LICENSE](https://github.com/maxkrivich/SlowLoris/blob/master/LICENSE) file for details\n\nCopyright (c) 2017-2020 Maxim Krivich\n\n[here]: <https://en.wikipedia.org/wiki/Slowloris_(computer_security)>\n[bugs]: <https://github.com/maxkrivich/SlowLoris/issues>\n[suggestions]: <https://github.com/maxkrivich/SlowLoris/issues>\n',
-    'author': 'Maxim Krivich',
-    'author_email': 'maxkrivich@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/maxkrivich/SlowLoris',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+More information about the attack you can find [here].
 
+### Installation
+
+#### PyPi
+
+For installation through the PyPI:
+
+```sh
+$ pip install pyslowloris==2.0.1
+```
+This method is prefered for installation of the most recent stable release.
+
+
+#### Source-code
+
+For installation through the source-code for local development:
+```sh
+$ git clone https://github.com/[username]/SlowLoris.git
+$ cd SlowLoris
+$ pip install poetry
+$ pyenv install 3.8.3
+$ pyenv local 3.8.3
+$ poetry env use 3.8.3
+```
+
+### Basic Usage
+
+Available command list:
+
+```sh
+$ slowloris --help
+usage: slowloris [-h] -u URL [-c CONNECTION_COUNT] [-s]
+
+Asynchronous Python implementation of SlowLoris attack
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -u URL, --url URL     Link to a web server (http://google.com) - str
+  -c CONNECTION_COUNT, --connection-count CONNECTION_COUNT
+                        Count of active connections (default value is 247) - int
+  -s, --silent          Ignore all of the errors [pure attack mode] - bool
+```
+
+### Docker usage
+
+#### Download image from Docker Hub
+
+Pull the image from [Docker Hub](https://hub.docker.com/r/maxkrivich/pyslowloris/) and run a container:
+
+```bash
+$ docker pull maxkrivich/pyslowloris
+$ docker run --rm -it maxkrivich/pyslowloris [-h] [-u URL] [-c CONNECTION_COUNT] [-s SILENT]
+```
+
+#### Build image from source-code
+
+Also you can build image from [Dockerfile](https://github.com/maxkrivich/SlowLoris/blob/master/Dockerfile) and run a container:
+
+```bash
+$ docker build -t pyslowloris .
+$ docker run --rm -it pyslowloris [-h] [-u URL] [-c CONNECTION_COUNT] [-s SILENT]
+```
+
+**Note:** *Don't forget about 'sudo'!*
+
+
+
+### Example of usage
+
+#### How to use module through Python API
+Here is an example of usage
+
+```python
+from pyslowloris import HostAddress, SlowLorisAttack
+
+url = HostAddress.from_url("http://kpi.ua")
+connections_count = 100
+
+loris = SlowLorisAttack(url, connections_count, silent=True)
+loris.start()
+```
+
+#### How to use module via CLI
+
+The following command helps to use module from command line
+
+```sh
+$ slowloris -u http://kpi.ua/ -c 100 -s
+```
+###### stop execution: Ctrl + C
+
+
+
+### Testing
+
+#### Testing with real apache server
+
+```bash
+$ docker-compose up web_server -d
+$ .....
+```
+
+#### Module-tests
+```bash
+$ make pytest
+```
+
+### Bugs, issues and contributing
+
+If you find [bugs] or have [suggestions] about improving the module, don't hesitate to contact me.
+
+### License
+
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/maxkrivich/SlowLoris/blob/master/LICENSE) file for details
+
+Copyright (c) 2017-2020 Maxim Krivich
+
+[here]: <https://en.wikipedia.org/wiki/Slowloris_(computer_security)>
+[bugs]: <https://github.com/maxkrivich/SlowLoris/issues>
+[suggestions]: <https://github.com/maxkrivich/SlowLoris/issues>
 
-setup(**setup_kwargs)
```

