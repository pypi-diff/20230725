# Comparing `tmp/makenew_pypackage-4.1.1.tar.gz` & `tmp/makenew_pypackage-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makenew_pypackage-4.1.1.tar", max compression
+gzip compressed data, was "makenew_pypackage-4.2.0.tar", max compression
```

## Comparing `makenew_pypackage-4.1.1.tar` & `makenew_pypackage-4.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1079 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/LICENSE.txt
--rw-r--r--   0        0        0     6886 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/README.rst
--rw-r--r--   0        0        0       46 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/makenew_pypackage/__init__.py
--rw-r--r--   0        0        0       56 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/makenew_pypackage/todo.py
--rw-r--r--   0        0        0      156 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/makenew_pypackage/todo_test.py
--rw-r--r--   0        0        0      589 2023-01-29 00:11:16.900909 makenew_pypackage-4.1.1/pyproject.toml
--rw-r--r--   0        0        0     7764 1970-01-01 00:00:00.000000 makenew_pypackage-4.1.1/setup.py
--rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 makenew_pypackage-4.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     6865 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/README.rst
+-rw-r--r--   0        0        0       46 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/__init__.py
+-rw-r--r--   0        0        0       56 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/todo.py
+-rw-r--r--   0        0        0      156 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/makenew_pypackage/todo_test.py
+-rw-r--r--   0        0        0      615 2023-07-25 18:11:21.197274 makenew_pypackage-4.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7427 1970-01-01 00:00:00.000000 makenew_pypackage-4.2.0/PKG-INFO
```

### Comparing `makenew_pypackage-4.1.1/LICENSE.txt` & `makenew_pypackage-4.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `makenew_pypackage-4.1.1/README.rst` & `makenew_pypackage-4.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,23 +24,23 @@
 
 - Publishing to PyPI_.
 - Secure dependency management with Poetry_.
 - Linting with Pylint_.
 - Uncompromising code formatting with Black_.
 - pytest_ helps you write better programs.
 - Code coverage reporting with Codecov_.
-- Continuous testing and deployment with `GitHub Actions`_.
+- Continuous testing and deployment with `GitHub Actions`__.
 - `Keep a CHANGELOG`_.
 - Consistent coding with EditorConfig_.
 - Badges from Shields.io_.
 
 .. _Black: https://black.readthedocs.io/en/stable/
 .. _Codecov: https://codecov.io/
 .. _EditorConfig: https://editorconfig.org/
-.. _GitHub Actions: https://github.com/features/actions
+.. __: https://github.com/features/actions
 .. _Keep a CHANGELOG: https://keepachangelog.com/
 .. _PyPI: https://pypi.python.org/pypi
 .. _Pylint: https://www.pylint.org/
 .. _Shields.io: https://shields.io/
 .. _pytest: https://docs.pytest.org/
 
 Bootstrapping a New Project
@@ -159,22 +159,22 @@
     $ make watch
 
 Primary development tasks are defined in the `Makefile`.
 
 Source Code
 ~~~~~~~~~~~
 
-The `source code`_ is hosted on GitHub.
+The `source code`__ is hosted on GitHub.
 Clone the project with
 
 ::
 
     $ git clone https://github.com/makenew/pypackage.git
 
-.. _source code: https://github.com/makenew/pypackage
+.. __: https://github.com/makenew/pypackage
 
 Requirements
 ~~~~~~~~~~~~
 
 You will need `Python 3`_ and Poetry_.
 
 Install the development dependencies with
```

### Comparing `makenew_pypackage-4.1.1/pyproject.toml` & `makenew_pypackage-4.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "makenew-pypackage"
-version = "4.1.1"
+version = "4.2.0"
 description = "Package skeleton for a Python module."
 authors = ["Evan Sosenko <razorx@evansosenko.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/makenew/pypackage"
 repository = "https://github.com/makenew/pypackage"
 
 [tool.poetry.dependencies]
 python = "^3.10.0"
 
-[tool.poetry.dev-dependencies]
-black = "^22.3.0"
+[tool.poetry.group.dev.dependencies]
+black = "^23.7.0"
 pylint = "^2.4.0"
 pytest = "^7.1.1"
 pytest-cov = "^4.0.0"
 pytest-runner = "^6.0.0"
 pytest-watch = "^4.2.0"
+rstcheck = "^6.1.2"
 
 [build-system]
 requires = ["poetry>=1.2"]
 build-backend = "poetry.masonry.api"
```

### Comparing `makenew_pypackage-4.1.1/setup.py` & `makenew_pypackage-4.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,298 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: makenew-pypackage
+Version: 4.2.0
+Summary: Package skeleton for a Python module.
+Home-page: https://github.com/makenew/pypackage
+License: MIT
+Author: Evan Sosenko
+Author-email: razorx@evansosenko.com
+Requires-Python: >=3.10.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/makenew/pypackage
+Description-Content-Type: text/x-rst
 
-packages = \
-['makenew_pypackage']
+Python Package Skeleton
+=======================
 
-package_data = \
-{'': ['*']}
+|PyPI| |GitHub Actions|
 
-setup_kwargs = {
-    'name': 'makenew-pypackage',
-    'version': '4.1.1',
-    'description': 'Package skeleton for a Python module.',
-    'long_description': 'Python Package Skeleton\n=======================\n\n|PyPI| |GitHub Actions|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/makenew-pypackage.svg\n   :target: https://pypi.python.org/pypi/makenew-pypackage\n   :alt: PyPI\n.. |GitHub Actions| image:: https://github.com/makenew/pypackage/actions/workflows/check.yml/badge.svg\n   :target: https://github.com/makenew/pypackage/actions/workflows/check.yml\n   :alt: GitHub Actions\n\nPackage skeleton for a Python module.\n\nDescription\n-----------\n\nBootstrap a new Python_ package in less than a minute.\n\n.. _Python: https://www.python.org/\n\nFeatures\n~~~~~~~~\n\n- Publishing to PyPI_.\n- Secure dependency management with Poetry_.\n- Linting with Pylint_.\n- Uncompromising code formatting with Black_.\n- pytest_ helps you write better programs.\n- Code coverage reporting with Codecov_.\n- Continuous testing and deployment with `GitHub Actions`_.\n- `Keep a CHANGELOG`_.\n- Consistent coding with EditorConfig_.\n- Badges from Shields.io_.\n\n.. _Black: https://black.readthedocs.io/en/stable/\n.. _Codecov: https://codecov.io/\n.. _EditorConfig: https://editorconfig.org/\n.. _GitHub Actions: https://github.com/features/actions\n.. _Keep a CHANGELOG: https://keepachangelog.com/\n.. _PyPI: https://pypi.python.org/pypi\n.. _Pylint: https://www.pylint.org/\n.. _Shields.io: https://shields.io/\n.. _pytest: https://docs.pytest.org/\n\nBootstrapping a New Project\n~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\n1. Create an empty (**non-initialized**) repository on GitHub.\n2. Clone the main branch of this repository with\n\n   ::\n\n       $ git clone --single-branch https://github.com/makenew/pypackage.git new-pypackage\n       $ cd new-pypackage\n\n   Optionally, reset to the latest\n   `release <https://github.com/makenew/pypackage/releases>`__ with\n\n   ::\n\n       $ git reset --hard <version-tag>\n\n3. Run\n\n   ::\n\n       $ ./makenew.sh\n\n   This will replace the boilerplate, delete itself,\n   remove the git remote, remove upstream tags,\n   and stage changes for commit.\n\n4. Create the required GitHub repository secrets\n5. Review, commit, and push the changes to GitHub with\n\n   ::\n\n     $ git diff --cached\n     $ git commit -m "Replace makenew boilerplate"\n     $ git remote add origin git@github.com:<user>/<new-pypackage>.git\n     $ git push -u origin main\n\n6. Ensure the GitHub action passes,\n   then publish the initial version of the package with\n\n   ::\n\n     $ poetry install\n     $ poetry version patch\n     $ make version\n\nUpdating\n~~~~~~~~\n\nIf you want to pull in future updates from this skeleton,\nyou can fetch and merge in changes from this repository.\n\nAdd this as a new remote with\n\n::\n\n    $ git remote rename origin upstream\n\nand then configure your ``origin`` branch as normal.\n\nOtherwise, add this as a new remote with\n\n::\n\n    $ git remote add upstream git@github.com:makenew/pypackage.git\n\nYou can then fetch and merge changes with\n\n::\n\n    $ git fetch --no-tags upstream\n    $ git merge upstream/main\n\nChangelog\n^^^^^^^^^\n\nNote that ``CHANGELOG.md`` is just a template for this skeleton. The\nactual changes for this project are documented in the commit history and\nsummarized under\n`Releases <https://github.com/makenew/pypackage/releases>`__.\n\nInstallation\n------------\n\nThis package is registered on the `Python Package Index (PyPI)`_\nas makenew-pypackage_.\n\nInstall it with\n\n::\n\n    $ poetry add makenew-pypackage\n\n.. _makenew-pypackage: https://pypi.python.org/pypi/makenew-pypackage\n.. _Python Package Index (PyPI): https://pypi.python.org/\n\nDevelopment and Testing\n-----------------------\n\nQuickstart\n~~~~~~~~~~\n\n::\n\n    $ git clone https://github.com/makenew/pypackage.git\n    $ cd pypackage\n    $ poetry install\n\nRun each command below in a separate terminal window:\n\n::\n\n    $ make watch\n\nPrimary development tasks are defined in the `Makefile`.\n\nSource Code\n~~~~~~~~~~~\n\nThe `source code`_ is hosted on GitHub.\nClone the project with\n\n::\n\n    $ git clone https://github.com/makenew/pypackage.git\n\n.. _source code: https://github.com/makenew/pypackage\n\nRequirements\n~~~~~~~~~~~~\n\nYou will need `Python 3`_ and Poetry_.\n\nInstall the development dependencies with\n\n::\n\n    $ poetry install\n\n.. _Poetry: https://poetry.eustace.io/\n.. _Python 3: https://www.python.org/\n\nTests\n~~~~~\n\nLint code with\n\n::\n\n    $ make lint\n\n\nRun tests with\n\n::\n\n    $ make test\n\nRun tests on changes with\n\n::\n\n    $ make watch\n\nPublishing\n~~~~~~~~~~\n\nUse the `poetry version`_ command to release a new version.\nThen run `make version` to commit and push a new git tag\nwhich will trigger a GitHub action.\n\nPublishing may be triggered using a `workflow_dispatch on GitHub Actions`_.\n\n.. _Poetry version: https://python-poetry.org/docs/cli/#version\n.. _workflow_dispatch on GitHub Actions: https://github.com/makenew/pypackage/actions?query=workflow%3Aversion\n\nGitHub Actions\n--------------\n\n*GitHub Actions should already be configured: this section is for reference only.*\n\nThe following repository secrets must be set on GitHub Actions.\n\n- ``PYPI_API_TOKEN``: API token for publishing on PyPI.\n\nThese must be set manually.\n\nSecrets for Optional GitHub Actions\n~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~\n\nThe version and format GitHub actions\nrequire a user with write access to the repository\nincluding access to read and write packages.\nSet these additional secrets to enable the action:\n\n- ``GH_TOKEN``: A personal access token for the user.\n- ``GIT_USER_NAME``: The name to set for Git commits.\n- ``GIT_USER_EMAIL``: The email to set for Git commits.\n- ``GPG_PRIVATE_KEY``: The `GPG private key`_.\n- ``GPG_PASSPHRASE``: The GPG key passphrase.\n\n.. _GPG private key: https://github.com/marketplace/actions/import-gpg#prerequisites\n\nContributing\n------------\n\nPlease submit and comment on bug reports and feature requests.\n\nTo submit a patch:\n\n1. Fork it (https://github.com/makenew/pypackage/fork).\n2. Create your feature branch (`git checkout -b my-new-feature`).\n3. Make changes.\n4. Commit your changes (`git commit -am \'Add some feature\'`).\n5. Push to the branch (`git push origin my-new-feature`).\n6. Create a new Pull Request.\n\nLicense\n-------\n\nThis Python package is licensed under the MIT license.\n\nWarranty\n--------\n\nThis software is provided by the copyright holders and contributors "as is" and\nany express or implied warranties, including, but not limited to, the implied\nwarranties of merchantability and fitness for a particular purpose are\ndisclaimed. In no event shall the copyright holder or contributors be liable for\nany direct, indirect, incidental, special, exemplary, or consequential damages\n(including, but not limited to, procurement of substitute goods or services;\nloss of use, data, or profits; or business interruption) however caused and on\nany theory of liability, whether in contract, strict liability, or tort\n(including negligence or otherwise) arising in any way out of the use of this\nsoftware, even if advised of the possibility of such damage.\n',
-    'author': 'Evan Sosenko',
-    'author_email': 'razorx@evansosenko.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/makenew/pypackage',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.10.0,<4.0.0',
-}
+.. |PyPI| image:: https://img.shields.io/pypi/v/makenew-pypackage.svg
+   :target: https://pypi.python.org/pypi/makenew-pypackage
+   :alt: PyPI
+.. |GitHub Actions| image:: https://github.com/makenew/pypackage/actions/workflows/check.yml/badge.svg
+   :target: https://github.com/makenew/pypackage/actions/workflows/check.yml
+   :alt: GitHub Actions
 
+Package skeleton for a Python module.
+
+Description
+-----------
+
+Bootstrap a new Python_ package in less than a minute.
+
+.. _Python: https://www.python.org/
+
+Features
+~~~~~~~~
+
+- Publishing to PyPI_.
+- Secure dependency management with Poetry_.
+- Linting with Pylint_.
+- Uncompromising code formatting with Black_.
+- pytest_ helps you write better programs.
+- Code coverage reporting with Codecov_.
+- Continuous testing and deployment with `GitHub Actions`__.
+- `Keep a CHANGELOG`_.
+- Consistent coding with EditorConfig_.
+- Badges from Shields.io_.
+
+.. _Black: https://black.readthedocs.io/en/stable/
+.. _Codecov: https://codecov.io/
+.. _EditorConfig: https://editorconfig.org/
+.. __: https://github.com/features/actions
+.. _Keep a CHANGELOG: https://keepachangelog.com/
+.. _PyPI: https://pypi.python.org/pypi
+.. _Pylint: https://www.pylint.org/
+.. _Shields.io: https://shields.io/
+.. _pytest: https://docs.pytest.org/
+
+Bootstrapping a New Project
+~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+1. Create an empty (**non-initialized**) repository on GitHub.
+2. Clone the main branch of this repository with
+
+   ::
+
+       $ git clone --single-branch https://github.com/makenew/pypackage.git new-pypackage
+       $ cd new-pypackage
+
+   Optionally, reset to the latest
+   `release <https://github.com/makenew/pypackage/releases>`__ with
+
+   ::
+
+       $ git reset --hard <version-tag>
+
+3. Run
+
+   ::
+
+       $ ./makenew.sh
+
+   This will replace the boilerplate, delete itself,
+   remove the git remote, remove upstream tags,
+   and stage changes for commit.
+
+4. Create the required GitHub repository secrets
+5. Review, commit, and push the changes to GitHub with
+
+   ::
+
+     $ git diff --cached
+     $ git commit -m "Replace makenew boilerplate"
+     $ git remote add origin git@github.com:<user>/<new-pypackage>.git
+     $ git push -u origin main
+
+6. Ensure the GitHub action passes,
+   then publish the initial version of the package with
+
+   ::
+
+     $ poetry install
+     $ poetry version patch
+     $ make version
+
+Updating
+~~~~~~~~
+
+If you want to pull in future updates from this skeleton,
+you can fetch and merge in changes from this repository.
+
+Add this as a new remote with
+
+::
+
+    $ git remote rename origin upstream
+
+and then configure your ``origin`` branch as normal.
+
+Otherwise, add this as a new remote with
+
+::
+
+    $ git remote add upstream git@github.com:makenew/pypackage.git
+
+You can then fetch and merge changes with
+
+::
+
+    $ git fetch --no-tags upstream
+    $ git merge upstream/main
+
+Changelog
+^^^^^^^^^
+
+Note that ``CHANGELOG.md`` is just a template for this skeleton. The
+actual changes for this project are documented in the commit history and
+summarized under
+`Releases <https://github.com/makenew/pypackage/releases>`__.
+
+Installation
+------------
+
+This package is registered on the `Python Package Index (PyPI)`_
+as makenew-pypackage_.
+
+Install it with
+
+::
+
+    $ poetry add makenew-pypackage
+
+.. _makenew-pypackage: https://pypi.python.org/pypi/makenew-pypackage
+.. _Python Package Index (PyPI): https://pypi.python.org/
+
+Development and Testing
+-----------------------
+
+Quickstart
+~~~~~~~~~~
+
+::
+
+    $ git clone https://github.com/makenew/pypackage.git
+    $ cd pypackage
+    $ poetry install
+
+Run each command below in a separate terminal window:
+
+::
+
+    $ make watch
+
+Primary development tasks are defined in the `Makefile`.
+
+Source Code
+~~~~~~~~~~~
+
+The `source code`__ is hosted on GitHub.
+Clone the project with
+
+::
+
+    $ git clone https://github.com/makenew/pypackage.git
+
+.. __: https://github.com/makenew/pypackage
+
+Requirements
+~~~~~~~~~~~~
+
+You will need `Python 3`_ and Poetry_.
+
+Install the development dependencies with
+
+::
+
+    $ poetry install
+
+.. _Poetry: https://poetry.eustace.io/
+.. _Python 3: https://www.python.org/
+
+Tests
+~~~~~
+
+Lint code with
+
+::
+
+    $ make lint
+
+
+Run tests with
+
+::
+
+    $ make test
+
+Run tests on changes with
+
+::
+
+    $ make watch
+
+Publishing
+~~~~~~~~~~
+
+Use the `poetry version`_ command to release a new version.
+Then run `make version` to commit and push a new git tag
+which will trigger a GitHub action.
+
+Publishing may be triggered using a `workflow_dispatch on GitHub Actions`_.
+
+.. _Poetry version: https://python-poetry.org/docs/cli/#version
+.. _workflow_dispatch on GitHub Actions: https://github.com/makenew/pypackage/actions?query=workflow%3Aversion
+
+GitHub Actions
+--------------
+
+*GitHub Actions should already be configured: this section is for reference only.*
+
+The following repository secrets must be set on GitHub Actions.
+
+- ``PYPI_API_TOKEN``: API token for publishing on PyPI.
+
+These must be set manually.
+
+Secrets for Optional GitHub Actions
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The version and format GitHub actions
+require a user with write access to the repository
+including access to read and write packages.
+Set these additional secrets to enable the action:
+
+- ``GH_TOKEN``: A personal access token for the user.
+- ``GIT_USER_NAME``: The name to set for Git commits.
+- ``GIT_USER_EMAIL``: The email to set for Git commits.
+- ``GPG_PRIVATE_KEY``: The `GPG private key`_.
+- ``GPG_PASSPHRASE``: The GPG key passphrase.
+
+.. _GPG private key: https://github.com/marketplace/actions/import-gpg#prerequisites
+
+Contributing
+------------
+
+Please submit and comment on bug reports and feature requests.
+
+To submit a patch:
+
+1. Fork it (https://github.com/makenew/pypackage/fork).
+2. Create your feature branch (`git checkout -b my-new-feature`).
+3. Make changes.
+4. Commit your changes (`git commit -am 'Add some feature'`).
+5. Push to the branch (`git push origin my-new-feature`).
+6. Create a new Pull Request.
+
+License
+-------
+
+This Python package is licensed under the MIT license.
+
+Warranty
+--------
+
+This software is provided by the copyright holders and contributors "as is" and
+any express or implied warranties, including, but not limited to, the implied
+warranties of merchantability and fitness for a particular purpose are
+disclaimed. In no event shall the copyright holder or contributors be liable for
+any direct, indirect, incidental, special, exemplary, or consequential damages
+(including, but not limited to, procurement of substitute goods or services;
+loss of use, data, or profits; or business interruption) however caused and on
+any theory of liability, whether in contract, strict liability, or tort
+(including negligence or otherwise) arising in any way out of the use of this
+software, even if advised of the possibility of such damage.
 
-setup(**setup_kwargs)
```

