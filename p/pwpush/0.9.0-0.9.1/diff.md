# Comparing `tmp/pwpush-0.9.0.tar.gz` & `tmp/pwpush-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwpush-0.9.0.tar", max compression
+gzip compressed data, was "pwpush-0.9.1.tar", max compression
```

## Comparing `pwpush-0.9.0.tar` & `pwpush-0.9.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1071 2021-08-20 21:05:30.110732 pwpush-0.9.0/LICENSE
--rw-r--r--   0        0        0     9626 2022-11-06 10:09:15.602585 pwpush-0.9.0/README.md
--rw-r--r--   0        0        0      432 2021-08-20 21:05:30.088281 pwpush-0.9.0/pwpush/__init__.py
--rw-r--r--   0        0        0    11745 2022-08-31 08:14:28.717976 pwpush-0.9.0/pwpush/__main__.py
--rw-r--r--   0        0        0     4821 2022-08-31 08:14:28.718237 pwpush-0.9.0/pwpush/commands/config.py
--rw-r--r--   0        0        0     3181 2022-08-31 08:14:28.718457 pwpush-0.9.0/pwpush/options.py
--rw-r--r--   0        0        0        0 2021-08-20 21:05:30.091678 pwpush-0.9.0/pwpush/py.typed
--rw-r--r--   0        0        0     3053 2022-11-06 10:09:15.609164 pwpush-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    10806 2022-11-06 10:11:18.106773 pwpush-0.9.0/setup.py
--rw-r--r--   0        0        0    10768 2022-11-06 10:11:18.107717 pwpush-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2021-08-20 21:05:30.110732 pwpush-0.9.1/LICENSE
+-rw-r--r--   0        0        0     9702 2023-07-24 21:59:40.082265 pwpush-0.9.1/README.md
+-rw-r--r--   0        0        0      432 2021-08-20 21:05:30.088281 pwpush-0.9.1/pwpush/__init__.py
+-rw-r--r--   0        0        0    11811 2023-07-24 21:40:38.881003 pwpush-0.9.1/pwpush/__main__.py
+-rw-r--r--   0        0        0     4821 2022-08-31 08:14:28.718237 pwpush-0.9.1/pwpush/commands/config.py
+-rw-r--r--   0        0        0     3224 2022-11-14 09:47:14.551927 pwpush-0.9.1/pwpush/options.py
+-rw-r--r--   0        0        0        0 2021-08-20 21:05:30.091678 pwpush-0.9.1/pwpush/py.typed
+-rw-r--r--   0        0        0     3135 2023-07-24 21:59:42.296319 pwpush-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10843 1970-01-01 00:00:00.000000 pwpush-0.9.1/PKG-INFO
```

### Comparing `pwpush-0.9.0/LICENSE` & `pwpush-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.0/README.md` & `pwpush-0.9.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 It uses the JSON API of Password Pusher to create, view, retrieve and manage pushes.  It can do this anonymously or via the authenticated API.
 
 # Installation
 
 `pip install pwpush`
 
-* Required Python version >3.5
+* Required Python version >3.8
 
 # Quickstart
 
 ## pwpush.com
 
 ```sh
 # Push a password to pwpush.com
@@ -129,20 +129,20 @@
 User config is saved in '/Users/pglombardo/Library/Application Support/pwpush/config.ini'
 ```
 
 # Screenshots
 
 ## Help
 
-![](https://disznc.s3.amazonaws.com/pwpush-cli-help.png)
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-help.png)
 
 ## List
 
-![](https://disznc.s3.amazonaws.com/pwpush-cli-list.png)
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-list.png)
 
 ## Audit
 
-![](https://disznc.s3.amazonaws.com/pwpush-cli-audit.png)
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-audit.png)
 
 ## Config
 
-![](https://disznc.s3.amazonaws.com/pwpush-cli-config.png)
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-config.png)
```

### Comparing `pwpush-0.9.0/pwpush/__main__.py` & `pwpush-0.9.1/pwpush/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 ) -> None:
     """
     Login to the registered Password Pusher instance.
 
     Your email and API token is required.
     Your API token is available at https://pwpush.com/en/users/token.
     """
-    r = requests.get(url + "/en/d/active", auth=(email, token))
+    r = requests.get(url + "/en/d/active", auth=(email, token), timeout=5)
 
     if r.status_code == 200:
         user_config["instance"]["url"] = url
         user_config["instance"]["email"] = email
         user_config["instance"]["token"] = token
         save_config()
         rprint()
@@ -351,25 +351,27 @@
     if valid_email and valid_token:
         auth_headers["X-User-Email"] = email
         auth_headers["X-User-Token"] = token
 
     if method == "GET":
         if debug:
             rprint(f"Making GET request to {url + path} with headers {auth_headers}")
-        return requests.get(url + path, headers=auth_headers)
+        return requests.get(url + path, headers=auth_headers, timeout=5)
     elif method == "POST":
         if debug:
             rprint(
                 f"Making JSON POST request to {url + path} with headers {auth_headers} and body {post_data}"
             )
-        return requests.post(url + path, headers=auth_headers, json=post_data)
+        return requests.post(
+            url + path, headers=auth_headers, json=post_data, timeout=5
+        )
     elif method == "DELETE":
         if debug:
             rprint(f"Making DELETE request to {url + path} with headers {auth_headers}")
-        return requests.delete(url + path, headers=auth_headers)
+        return requests.delete(url + path, headers=auth_headers, timeout=5)
 
 
 def json_output() -> Boolean:
     if cli_options["json"] == True or user_config["cli"]["json"] is True:
         return True
     return False
```

### Comparing `pwpush-0.9.0/pwpush/commands/config.py` & `pwpush-0.9.1/pwpush/commands/config.py`

 * *Files identical despite different names*

### Comparing `pwpush-0.9.0/pwpush/options.py` & `pwpush-0.9.1/pwpush/options.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,21 +38,22 @@
     """
     if os.path.exists(user_config_file) is True:
         user_config.read(user_config_file)
 
         validate_user_config()
     else:
         # No config file exists; Write out a new file with default settings
+        user_config.read_dict(default_config)
 
         # Write out default settings to a new config file
         if os.path.exists(user_config_dir) is False:
             Path.mkdir(user_config_dir)
 
         with open(user_config_file, "x") as file:
-            default_config.write(file)
+            user_config.write(file)
 
 
 def validate_user_config():
     """
     Validate `user_config` and assure that all default keys are set
     and available.
     """
```

### Comparing `pwpush-0.9.0/pyproject.toml` & `pwpush-0.9.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pwpush"
-version = "0.9.0"
+version = "0.9.1"
 description = "Command Line Interface to Password Pusher."
 readme = "README.md"
 authors = ["pwpush <pglombardo@hey.com>"]
 license = "MIT"
 repository = "https://github.com/pglombardo/pwpush"
 homepage = "https://github.com/pglombardo/pwpush"
 
@@ -20,46 +20,48 @@
 classifiers = [  #! Update me
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
+  "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.scripts]
 # Entry points for the package https://python-poetry.org/docs/pyproject/#scripts
 "pwpush" = "pwpush.__main__:app"
 
 [tool.poetry.dependencies]
-python = "^3.7"
-importlib_metadata = {version = "^4.5.0", python = "<3.8"}
-typer = {extras = ["all"], version = "^0.6.1"}
+python = ">=3.8,<4.0"
+importlib_metadata = {version = ">=4.5,<7.0", python = "<3.8"}
+typer = {extras = ["all"], version = ">=0.6.1,<0.10.0"}
 rich = "^12.5.1"
 requests = "^2.28.1"
 shellingham = "^1.5.0"
 python-dateutil = "^2.8.2"
 
 [tool.poetry.dev-dependencies]
 bandit = "^1.7.0"
 black = {version = ">=22.6.0", allow-prereleases = true}
 darglint = "^1.8.0"
-isort = {extras = ["colors"], version = "^5.9.3"}
-mypy = "^0.910"
-mypy-extensions = "^0.4.3"
-pre-commit = "^2.13.0"
+isort = {extras = ["colors"], version = "^5.11.5"}
+mypy = "^1.1"
+mypy-extensions = "^1.0.0"
+pre-commit = "^2.21.0"
 pydocstyle = "^6.1.1"
 pylint = "^2.9.6"
-pytest = "^6.2.4"
-pyupgrade = "^2.23.1"
-safety = "^1.10.3"
-ipdb = "^0.13.9"
+pytest = "^7.2.2"
+pyupgrade = "^3.3.1"
+safety = "^2.3.5"
+ipdb = "^0.13.13"
+ipython = "^8.12.2"
 
 [tool.black]
 # https://github.com/psf/black
 target-version = ["py37"]
 line-length = 88
 color = true
```

### Comparing `pwpush-0.9.0/setup.py` & `pwpush-0.9.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,177 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pwpush
+Version: 0.9.1
+Summary: Command Line Interface to Password Pusher.
+Home-page: https://github.com/pglombardo/pwpush
+License: MIT
+Author: pwpush
+Author-email: pglombardo@hey.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: importlib_metadata (>=4.5,<7.0) ; python_version < "3.8"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: shellingham (>=1.5.0,<2.0.0)
+Requires-Dist: typer[all] (>=0.6.1,<0.10.0)
+Project-URL: Repository, https://github.com/pglombardo/pwpush
+Description-Content-Type: text/markdown
 
-packages = \
-['pwpush', 'pwpush.commands']
+# pwpush
 
-package_data = \
-{'': ['*']}
+<div align="center">
 
-install_requires = \
-['python-dateutil>=2.8.2,<3.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'rich>=12.5.1,<13.0.0',
- 'shellingham>=1.5.0,<2.0.0',
- 'typer[all]>=0.6.1,<0.7.0']
-
-extras_require = \
-{':python_version < "3.8"': ['importlib_metadata>=4.5.0,<5.0.0']}
-
-entry_points = \
-{'console_scripts': ['pwpush = pwpush.__main__:app']}
-
-setup_kwargs = {
-    'name': 'pwpush',
-    'version': '0.9.0',
-    'description': 'Command Line Interface to Password Pusher.',
-    'long_description': '# pwpush\n\n<div align="center">\n\n[![Build status](https://github.com/pglombardo/pwpush-cli/workflows/build/badge.svg?branch=master&event=push)](https://github.com/pglombardo/pwpush-cli/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/pwpush.svg)](https://pypi.org/project/pwpush/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/pglombardo/pwpush-cli/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pglombardo/pwpush-cli/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/pglombardo/pwpush-cli/releases)\n[![License](https://img.shields.io/github/license/pglombardo/pwpush-cli)](https://github.com/pglombardo/pwpush/blob/master/LICENSE)\n\nCommand Line Interface to Password Pusher.\n  \n<strong>This utility is currently in pre-beta form.  Most core functionality exists and works but needs a bit of polishing.</strong>\n\n</div>\n\n# Overview\n\nThis command line utility exists to interface with [pwpush.com](https://pwpush.com) or any privately hosted instance of [Password Pusher](https://github.com/pglombardo/PasswordPusher).\n\nIt uses the JSON API of Password Pusher to create, view, retrieve and manage pushes.  It can do this anonymously or via the authenticated API.\n\n# Installation\n\n`pip install pwpush`\n\n* Required Python version >3.5\n\n# Quickstart\n\n## pwpush.com\n\n```sh\n# Push a password to pwpush.com\n> pwpush push mypassword\nhttps://pwpush.com/en/p/uzij1ybk6rol\n\n# Get JSON output instead\n> pwpush --json=true push mypassword\n{\'url\': \'https://pwpush.com/en/p/uzij1ybk6rol\'}\n```\n## Private Self Hosted Instance\n\n```sh\n# Point this tool to your privately hosted instance\n> pwpush config set --key url --value https://pwpush.mydomain.secure\n# ...and push away...\n> pwpush push mypassword\nhttps://pwpush.mydomain.secure/en/p/uzij1ybk6rol\n```\n\n## Authentication with API Token\n\nGet [the API token associated with your account](https://pwpush.com/en/users/token) and add it to the CLI configuration.\n\n```sh\n# Get your API token at [/en/users/token](https://pwpush.com/en/users/token)\n\n# Configure the CLI with your email and API token\n> pwpush config set --key email --value <pwpush login email>\n> pwpush config set --key token --value <api token from /en/users/token>\n\n# List active pushes in your dashboard\n> pwpush list\n\n=== Active Pushes:\n┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Secret URL Token   ┃ Note                   ┃ Views ┃ Days  ┃ Deletable by Viewer ┃ Retrieval Step ┃ Created                ┃\n┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ uzij1ybk6rol       │ Push prior to Digital  │ 6/100 │ 28/87 │ True                │ False          │ 10/08/2022, 11:55:49   │\n│                    │ Ocean migration 3      │       │       │                     │                │ UTC                    │\n│ sfoej1fwlfljwlf    │ Push prior to Digital  │ 0/100 │ 28/90 │ True                │ True           │ 10/08/2022, 11:55:19   │\n│                    │ Ocean migration 2      │       │       │                     │                │ UTC                    │\n└────────────────────┴────────────────────────┴───────┴───────┴─────────────────────┴────────────────┴────────────────────────┘\n\n# Get the audit log for a push\n> pwpush audit <secret url token>\n```\n\n## Show Configuration\n\n```\n> pwpush config show\n\n=== Instance Settings:\nSpecify your credentials and even your private Password Pusher instance here.\n\n┏━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Key   ┃ Value              ┃ Description                                                            ┃\n┡━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ URL   │ https://pwpush.com │ The Password Pusher instance to work with.                             │\n│ email │ Not Set            │ E-mail address of your account on Password Pusher.                     │\n│ token │ Not Set            │ API token from your account.  e.g. \'https://pwpush.com/en/users/token\' │\n└───────┴────────────────────┴────────────────────────────────────────────────────────────────────────┘\n\n=== Expiration Settings:\nPushes created with this tool will have these expiration settings.\n\nIf not specified, the application defaults will be used.\nCommand line options override these settings.  See \'pwpush push --help\'\n\n┏━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Key                 ┃ Value   ┃ Valid Values ┃ Description                                                      ┃\n┡━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ expire_after_days   │ Not Set │ 1-90         │ Number of days each push will be valid for.                      │\n│ expire_after_views  │ Not Set │ 1-100        │ Number of views each push will be valid for.                     │\n│ retrieval_step      │ Not Set │ true/false   │ Require users to perform a click through to retrieve a push.     │\n│ deletable_by_viewer │ Not Set │ true/false   │ Enables/disables a user from deleting a push payload themselves. │\n└─────────────────────┴─────────┴──────────────┴──────────────────────────────────────────────────────────────────┘\n\n=== CLI Settings:\nBehavior settings for this CLI.\n\nCommand line options override these settings.  See \'pwpush --help\'\n\n┏━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓\n┃ Key     ┃ Value ┃ Valid Values ┃ Description                      ┃\n┡━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩\n│ json    │ False │ true/false   │ CLI outputs results in JSON.     │\n│ verbose │ False │ true/false   │ More verbosity when appropriate. │\n└─────────┴───────┴──────────────┴──────────────────────────────────┘\n\nTo change the above the values see: \'pwpush config set --help\'\n\nUser config is saved in \'/Users/pglombardo/Library/Application Support/pwpush/config.ini\'\n```\n\n# Screenshots\n\n## Help\n\n![](https://disznc.s3.amazonaws.com/pwpush-cli-help.png)\n\n## List\n\n![](https://disznc.s3.amazonaws.com/pwpush-cli-list.png)\n\n## Audit\n\n![](https://disznc.s3.amazonaws.com/pwpush-cli-audit.png)\n\n## Config\n\n![](https://disznc.s3.amazonaws.com/pwpush-cli-config.png)\n',
-    'author': 'pwpush',
-    'author_email': 'pglombardo@hey.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/pglombardo/pwpush',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+[![Build status](https://github.com/pglombardo/pwpush-cli/workflows/build/badge.svg?branch=master&event=push)](https://github.com/pglombardo/pwpush-cli/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/pwpush.svg)](https://pypi.org/project/pwpush/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/pglombardo/pwpush-cli/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
 
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pglombardo/pwpush-cli/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/pglombardo/pwpush-cli/releases)
+[![License](https://img.shields.io/github/license/pglombardo/pwpush-cli)](https://github.com/pglombardo/pwpush/blob/master/LICENSE)
+
+Command Line Interface to Password Pusher.
+  
+<strong>This utility is currently in pre-beta form.  Most core functionality exists and works but needs a bit of polishing.</strong>
+
+</div>
+
+# Overview
+
+This command line utility exists to interface with [pwpush.com](https://pwpush.com) or any privately hosted instance of [Password Pusher](https://github.com/pglombardo/PasswordPusher).
+
+It uses the JSON API of Password Pusher to create, view, retrieve and manage pushes.  It can do this anonymously or via the authenticated API.
+
+# Installation
+
+`pip install pwpush`
+
+* Required Python version >3.8
+
+# Quickstart
+
+## pwpush.com
+
+```sh
+# Push a password to pwpush.com
+> pwpush push mypassword
+https://pwpush.com/en/p/uzij1ybk6rol
+
+# Get JSON output instead
+> pwpush --json=true push mypassword
+{'url': 'https://pwpush.com/en/p/uzij1ybk6rol'}
+```
+## Private Self Hosted Instance
+
+```sh
+# Point this tool to your privately hosted instance
+> pwpush config set --key url --value https://pwpush.mydomain.secure
+# ...and push away...
+> pwpush push mypassword
+https://pwpush.mydomain.secure/en/p/uzij1ybk6rol
+```
+
+## Authentication with API Token
+
+Get [the API token associated with your account](https://pwpush.com/en/users/token) and add it to the CLI configuration.
+
+```sh
+# Get your API token at [/en/users/token](https://pwpush.com/en/users/token)
+
+# Configure the CLI with your email and API token
+> pwpush config set --key email --value <pwpush login email>
+> pwpush config set --key token --value <api token from /en/users/token>
+
+# List active pushes in your dashboard
+> pwpush list
+
+=== Active Pushes:
+┏━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Secret URL Token   ┃ Note                   ┃ Views ┃ Days  ┃ Deletable by Viewer ┃ Retrieval Step ┃ Created                ┃
+┡━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ uzij1ybk6rol       │ Push prior to Digital  │ 6/100 │ 28/87 │ True                │ False          │ 10/08/2022, 11:55:49   │
+│                    │ Ocean migration 3      │       │       │                     │                │ UTC                    │
+│ sfoej1fwlfljwlf    │ Push prior to Digital  │ 0/100 │ 28/90 │ True                │ True           │ 10/08/2022, 11:55:19   │
+│                    │ Ocean migration 2      │       │       │                     │                │ UTC                    │
+└────────────────────┴────────────────────────┴───────┴───────┴─────────────────────┴────────────────┴────────────────────────┘
+
+# Get the audit log for a push
+> pwpush audit <secret url token>
+```
+
+## Show Configuration
+
+```
+> pwpush config show
+
+=== Instance Settings:
+Specify your credentials and even your private Password Pusher instance here.
+
+┏━━━━━━━┳━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Key   ┃ Value              ┃ Description                                                            ┃
+┡━━━━━━━╇━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ URL   │ https://pwpush.com │ The Password Pusher instance to work with.                             │
+│ email │ Not Set            │ E-mail address of your account on Password Pusher.                     │
+│ token │ Not Set            │ API token from your account.  e.g. 'https://pwpush.com/en/users/token' │
+└───────┴────────────────────┴────────────────────────────────────────────────────────────────────────┘
+
+=== Expiration Settings:
+Pushes created with this tool will have these expiration settings.
+
+If not specified, the application defaults will be used.
+Command line options override these settings.  See 'pwpush push --help'
+
+┏━━━━━━━━━━━━━━━━━━━━━┳━━━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Key                 ┃ Value   ┃ Valid Values ┃ Description                                                      ┃
+┡━━━━━━━━━━━━━━━━━━━━━╇━━━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ expire_after_days   │ Not Set │ 1-90         │ Number of days each push will be valid for.                      │
+│ expire_after_views  │ Not Set │ 1-100        │ Number of views each push will be valid for.                     │
+│ retrieval_step      │ Not Set │ true/false   │ Require users to perform a click through to retrieve a push.     │
+│ deletable_by_viewer │ Not Set │ true/false   │ Enables/disables a user from deleting a push payload themselves. │
+└─────────────────────┴─────────┴──────────────┴──────────────────────────────────────────────────────────────────┘
+
+=== CLI Settings:
+Behavior settings for this CLI.
+
+Command line options override these settings.  See 'pwpush --help'
+
+┏━━━━━━━━━┳━━━━━━━┳━━━━━━━━━━━━━━┳━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
+┃ Key     ┃ Value ┃ Valid Values ┃ Description                      ┃
+┡━━━━━━━━━╇━━━━━━━╇━━━━━━━━━━━━━━╇━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┩
+│ json    │ False │ true/false   │ CLI outputs results in JSON.     │
+│ verbose │ False │ true/false   │ More verbosity when appropriate. │
+└─────────┴───────┴──────────────┴──────────────────────────────────┘
+
+To change the above the values see: 'pwpush config set --help'
+
+User config is saved in '/Users/pglombardo/Library/Application Support/pwpush/config.ini'
+```
+
+# Screenshots
+
+## Help
+
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-help.png)
+
+## List
+
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-list.png)
+
+## Audit
+
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-audit.png)
+
+## Config
+
+![](https://pwpush.fra1.cdn.digitaloceanspaces.com/cli/pwpush-cli-config.png)
 
-setup(**setup_kwargs)
```

