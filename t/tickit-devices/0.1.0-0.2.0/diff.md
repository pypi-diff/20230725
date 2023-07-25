# Comparing `tmp/tickit-devices-0.1.0.tar.gz` & `tmp/tickit-devices-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickit-devices-0.1.0.tar", last modified: Tue Feb 21 11:28:43 2023, max compression
+gzip compressed data, was "tickit-devices-0.2.0.tar", last modified: Tue Jul 25 08:43:03 2023, max compression
```

## Comparing `tickit-devices-0.1.0.tar` & `tickit-devices-0.2.0.tar`

### file list

```diff
@@ -1,107 +1,181 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.562322 tickit-devices-0.1.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6502 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.gitremotes
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.566322 tickit-devices-0.1.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/docs/user/tutorials/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.562322 tickit-devices-0.1.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/examples/configs/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/examples/configs/synchrotron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/examples/configs/synchrotron_current.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/examples/configs/synchrotron_machine.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/examples/configs/synchrotron_topup.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/s03_configs/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/s03_configs/synchrotron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.562322 tickit-devices-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/src/tickit_devices/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/src/tickit_devices/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/src/tickit_devices/synchrotron/db_files/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/db_files/DCCT.db
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/db_files/FILL.db
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/db_files/MSTAT.db
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     8331 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_topup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/src/tickit_devices.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-21 11:28:43.000000 tickit-devices-0.1.0/src/tickit_devices.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:43.570322 tickit-devices-0.1.0/tests/synchrotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/synchrotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_current.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-02-21 11:28:33.000000 tickit-devices-0.1.0/tests/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.353947 tickit-devices-0.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.361947 tickit-devices-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.gitremotes
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6510 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.365947 tickit-devices-0.2.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/docs/user/tutorials/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.357947 tickit-devices-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/cryostream/cryo-tcp.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/eiger/eiger.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/femto/current-monitor.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/multi-ioc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/pneumatic/attns.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/examples/configs/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_current.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_machine.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/examples/configs/synchrotron/synchrotron_topup.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.369947 tickit-devices-0.2.0/s03_configs/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/s03_configs/synchrotron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.357947 tickit-devices-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12363 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/cryostream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/cryostream/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/dummy_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   514994 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/frame_sample
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/data/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15464 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/eiger_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/filewriter/filewriter_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.377947 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/monitor/monitor_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/eiger_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/eiger/stream/stream_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/femto.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/femto/record.db
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/db_files/filter1.db
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/pneumatic/pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.381947 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/DCCT.db
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/FILL.db
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/MSTAT.db
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7446 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8351 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_topup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.373947 tickit-devices-0.2.0/src/tickit_devices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 08:43:03.000000 tickit-devices-0.2.0/src/tickit_devices.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/cryostream/
+-rw-r--r--   0 runner    (1001) docker     (123)     9261 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/cryostream/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4542 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/cryostream/test_cryostream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/eiger/
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_filewriter_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_filewriter_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_monitor_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_monitor_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_stream_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/eiger/test_eiger_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/femto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/femto/test_femto.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/multi/test_multi_device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.385947 tickit-devices-0.2.0/tests/pneumatic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/pneumatic/test_pneumatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:43:03.389947 tickit-devices-0.2.0/tests/synchrotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_current.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-25 08:42:51.000000 tickit-devices-0.2.0/tests/test_cli.py
```

### Comparing `tickit-devices-0.1.0/.devcontainer/devcontainer.json` & `tickit-devices-0.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/CONTRIBUTING.rst` & `tickit-devices-0.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/actions/install_requirements/action.yml` & `tickit-devices-0.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/dependabot.yml` & `tickit-devices-0.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/pages/make_switcher.py` & `tickit-devices-0.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/workflows/code.yml` & `tickit-devices-0.2.0/.github/workflows/code.yml`

 * *Files 2% similar despite different names*

```diff
@@ -28,20 +28,20 @@
 
   test:
     if: github.event_name != 'pull_request' || github.event.pull_request.head.repo.full_name != github.repository
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"] # can add windows-latest, macos-latest
-        python: ["3.8", "3.9", "3.10"]
+        python: ["3.9", "3.10"]
         install: ["-e .[dev]"]
         # Make one version be non-editable to test both paths of version code
         include:
           - os: "ubuntu-latest"
-            python: "3.8"
+            python: "3.9"
             install: ".[dev]"
 
     runs-on: ${{ matrix.os }}
     env:
       # https://github.com/pytest-dev/pytest/issues/2042
       PY_IGNORE_IMPORTMISMATCH: "1"
 
@@ -89,14 +89,20 @@
 
       - name: Upload sdist and wheel as artifacts
         uses: actions/upload-artifact@v3
         with:
           name: dist
           path: dist
 
+      - name: Upload S03 configs as artifact
+        uses: actions/upload-artifact@v3
+        with:
+          name: s03_configs
+          path: s03_configs
+
       - name: Check for packaging errors
         run: pipx run twine check --strict dist/*
 
       - name: Install python packages
         uses: ./.github/actions/install_requirements
         with:
           python_version: ${{env.CONTAINER_PYTHON}}
@@ -139,27 +145,28 @@
       - name: Docker meta
         id: meta
         uses: docker/metadata-action@v4
         with:
           images: ${{ env.IMAGE_REPOSITORY }}
           tags: |
             type=ref,event=tag
+            type=ref,event=branch
             type=raw,value=latest
 
       - name: Set up Docker Buildx
         id: buildx
         uses: docker/setup-buildx-action@v2
 
       - name: Build runtime image
-        uses: docker/build-push-action@v3
+        uses: docker/build-push-action@v4
         with:
           build-args: |
             PIP_OPTIONS=-r lockfiles/requirements.txt dist/*.whl
-          push: ${{ github.event_name == 'push' && startsWith(github.ref, 'refs/tags') }}
-          load: ${{ ! (github.event_name == 'push' && startsWith(github.ref, 'refs/tags')) }}
+          push: ${{ github.event_name == 'push' && (startsWith(github.ref, 'refs/tags') || endsWith(github.ref, 'main'))}}
+          load: ${{ ! (github.event_name == 'push' && (startsWith(github.ref, 'refs/tags') || endsWith(github.ref, 'main'))) }}
           tags: ${{ steps.meta.outputs.tags }}
           labels: ${{ steps.meta.outputs.labels }}
           context: artifacts/
           file: ./Dockerfile
           # If you have a long docker build, uncomment the following to turn on caching
           # For short build times this makes it a little slower
           #cache-from: type=gha
```

### Comparing `tickit-devices-0.1.0/.github/workflows/docs.yml` & `tickit-devices-0.2.0/.github/workflows/docs.yml`

 * *Files 5% similar despite different names*

```diff
@@ -42,12 +42,12 @@
       - name: Write switcher.json
         run: python .github/pages/make_switcher.py --add $DOCS_VERSION ${{ github.repository }} .github/pages/switcher.json
 
       - name: Publish Docs to gh-pages
         if: github.event_name == 'push' && github.actor != 'dependabot[bot]'
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: peaceiris/actions-gh-pages@64b46b4226a4a12da2239ba3ea5aa73e3163c75b # v3.9.1
+        uses: peaceiris/actions-gh-pages@bd8c6b06eba6b3d25d72b7a1767993c0aeee42e7 # v3.9.2
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           publish_dir: .github/pages
           keep_files: true
```

### Comparing `tickit-devices-0.1.0/.github/workflows/docs_clean.yml` & `tickit-devices-0.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.github/workflows/linkcheck.yml` & `tickit-devices-0.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.gitignore` & `tickit-devices-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/.vscode/launch.json` & `tickit-devices-0.2.0/.vscode/launch.json`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 {
     // Use IntelliSense to learn about possible attributes.
     // Hover to view descriptions of existing attributes.
     // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
     "version": "0.2.0",
     "configurations": [
         {
+            "name": "Eiger",
+            "type": "python",
+            "request": "launch",
+            "module": "tickit",
+            "justMyCode": false,
+            "console": "integratedTerminal",
+            "args": [
+                "all",
+                "examples/configs/eiger/eiger.yaml"
+            ]
+        },
+        {
             "name": "Debug Unit Test",
             "type": "python",
             "request": "launch",
             "justMyCode": false,
             "program": "${file}",
             "purpose": [
                 "debug-test"
```

### Comparing `tickit-devices-0.1.0/.vscode/settings.json` & `tickit-devices-0.2.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/LICENSE` & `tickit-devices-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/PKG-INFO` & `tickit-devices-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit-devices
-Version: 0.1.0
+Version: 0.2.0
 Summary: Devices for tickit, an event-based device simulation framework
 Author-email: Abigail Emery <abigail.emery@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/dls-controls/tickit-devices
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 tickit-devices
 ===============
 
@@ -227,14 +226,22 @@
 PyPI           ``pip install tickit-devices``
 Source code    https://github.com/dls-controls/tickit-devices
 Documentation  https://dls-controls.github.io/tickit-devices
 Releases       https://github.com/dls-controls/tickit-devices/releases
 ============== ==============================================================
 
 
+Safety Note
+------------------------------------
+These devices mimic real synchrotron devices and there is the potential for conflict with the real PVs if this is run on the same port as EPICS (5064).
+If using this simulation to test software, set your ``EPICS_CA_SERVER_PORT`` environment variable to something nonstandard, e.g. 5065 or greater, so that your 
+tests are not confused between these and the real PVs. The `S03 <https://gitlab.diamond.ac.uk/controls/python3/s03_utils>`_ startup scripts manage the setting of
+these ports automatically, so if you are using this as part of S03 you won't need to change anything. Do not run this simulation on a beamline controls machine!
+
+
 Adding devices to the S03 simulation
 ------------------------------------
 To add a device to s03, the config file required to run the tickit simulation should be present in ``s03_configs``.
 Only changes pushed to main will be built into the ``tickit-devices`` image that s03 pulls from. Once the 
 image has been built with the new device and config, follow the instructions `here <https://gitlab.diamond.ac.uk/controls/python3/s03_utils>`_
 to include it in S03.
 
@@ -247,15 +254,15 @@
     :target: https://github.com/dls-controls/tickit-devices/actions/workflows/docs.yml
     :alt: Docs CI
 
 .. |coverage| image:: https://codecov.io/gh/dls-controls/tickit-devices/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dls-controls/tickit-devices
     :alt: Test Coverage
 
-.. |pypi_version| image:: https://img.shields.io/pypi/v/python3-pip-skeleton.svg
+.. |pypi_version| image:: https://img.shields.io/pypi/v/tickit-devices.svg
     :target: https://pypi.org/project/tickit-devices
     :alt: Latest PyPI version
 
 .. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
     :target: https://opensource.org/licenses/Apache-2.0
     :alt: Apache License
```

### Comparing `tickit-devices-0.1.0/docs/conf.py` & `tickit-devices-0.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `tickit-devices-0.2.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/explanations/decisions.rst` & `tickit-devices-0.2.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/build-docs.rst` & `tickit-devices-0.2.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/lint.rst` & `tickit-devices-0.2.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/make-release.rst` & `tickit-devices-0.2.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/pin-requirements.rst` & `tickit-devices-0.2.0/docs/developer/how-to/pin-requirements.rst`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 The files are created using ``pip freeze`` and will contain a full list
 of the dependencies and sub-dependencies with pinned versions.
 
 You can download any of these files by clicking on them. It is best to use
 the one that ran with the lowest Python version as this is more likely to
 be compatible with all the versions of Python in the test matrix.
-i.e. ``requirements-test-ubuntu-latest-3.8.txt`` in this example.
+i.e. ``requirements-test-ubuntu-latest-3.9.txt`` in this example.
 
 Applying the lock file
 ----------------------
 
 To apply a lockfile:
 
 - copy the requirements file you have downloaded to the root of your
```

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/test-container.rst` & `tickit-devices-0.2.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/how-to/update-tools.rst` & `tickit-devices-0.2.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/index.rst` & `tickit-devices-0.2.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/reference/standards.rst` & `tickit-devices-0.2.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/developer/tutorials/dev-install.rst` & `tickit-devices-0.2.0/docs/developer/tutorials/dev-install.rst`

 * *Files 18% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     $ git clone git://github.com/dls-controls/tickit-devices.git
 
 Install dependencies
 --------------------
 
 You can choose to either develop on the host machine using a `venv` (which
-requires python 3.8 or later) or to run in a container under `VSCode
+requires python 3.9 or later) or to run in a container under `VSCode
 <https://code.visualstudio.com/>`_
 
 .. tab-set::
 
     .. tab-item:: Local virtualenv
 
         .. code::
```

### Comparing `tickit-devices-0.1.0/docs/images/dls-favicon.ico` & `tickit-devices-0.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/images/dls-logo.svg` & `tickit-devices-0.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/index.rst` & `tickit-devices-0.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/user/explanations/docs-structure.rst` & `tickit-devices-0.2.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/user/index.rst` & `tickit-devices-0.2.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/docs/user/tutorials/installation.rst` & `tickit-devices-0.2.0/docs/user/tutorials/installation.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Installation
 ============
 
 Check your version of python
 ----------------------------
 
-You will need python 3.8 or later. You can check your version of python by
+You will need python 3.9 or later. You can check your version of python by
 typing into a terminal::
 
     $ python3 --version
 
 
 Create a virtual environment
 ----------------------------
```

### Comparing `tickit-devices-0.1.0/pyproject.toml` & `tickit-devices-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,26 +3,29 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tickit-devices"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 description = "Devices for tickit, an event-based device simulation framework"
 dependencies = [
-    "tickit"
-] 
+    "tickit>=0.3",
+    "typing_extensions",
+    "softioc",
+    "pydantic>1",
+    "apischema"
+]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
     "black",
     "mypy",
     "flake8-isort",
     "Flake8-pyproject",
@@ -51,14 +54,16 @@
 [project.urls]
 GitHub = "https://github.com/dls-controls/tickit-devices"
 
 [[project.authors]] # Further authors may be added by duplicating this section
 email = "abigail.emery@diamond.ac.uk"
 name = "Abigail Emery"
 
+[tool.setuptools.package-data]
+tickit_devices = ["**/frame_sample"]
 
 [tool.setuptools_scm]
 write_to = "src/tickit_devices/_version.py"
 
 [tool.mypy]
 ignore_missing_imports = true # Ignore missing stubs in imported modules
 
@@ -80,15 +85,14 @@
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
 addopts = """
     --tb=native -vv --doctest-modules --doctest-glob="*.rst"
     --cov=tickit-devices --cov-report term --cov-report xml:cov.xml
     """
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = [
-    "error",
     "ignore::ImportWarning" # Ongoing issue in six, which is used by aiokafa https://github.com/benjaminp/six/issues/368
 ]
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/tickit-devices.coverage"
```

### Comparing `tickit-devices-0.1.0/src/tickit_devices/synchrotron/db_files/MSTAT.db` & `tickit-devices-0.2.0/src/tickit_devices/synchrotron/db_files/MSTAT.db`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #Real world PV= CS-CS-MSTAT-01:MODE
-record (mbbi, "BL03S-CS-CS-MSTAT-01:MODE")
+record (mbbi, "CS-CS-MSTAT-01:MODE")
 {
     field (SCAN, "Passive")
     field (DESC, "Mode")
     field (ZRST, "Shutdown")
     field (ONST, "Injection")
     field (TWST, "No Beam")
     field (THST, "Mach. Dev.")
```

### Comparing `tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_current.py` & `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_current.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from dataclasses import dataclass
-from typing import Optional
+import pathlib
+from typing import Optional, TypedDict
 
+import pydantic.v1.dataclasses
 from softioc import builder
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.epicsadapter import EpicsAdapter
 from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.adapter import Server
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 
 class SynchrotronCurrentDevice(Device):
     """Device to simulate the ring current signal value from the synchrotron.
 
     This SynchrotronCurrentDevice simulates only a single signal that can be read,
     the beam current.The real world pv for this current is SR-DI-DCCT-01:SIGNAL.
@@ -153,33 +153,33 @@
     device: SynchrotronCurrentDevice
 
     def on_db_load(self) -> None:
         """Link loaded in record with getter for device."""
         self.link_input_on_interrupt(builder.aIn("SIGNAL"), self.device.get_current)
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class SynchrotronCurrent(ComponentConfig):
     """Synchrotron current component."""
 
     initial_current: Optional[float]
     callback_period: int = int(1e9)
     host: str = "localhost"
     port: int = 25565
     format: ByteFormat = ByteFormat(b"%b\r\n")
-    db_file: str = "src/tickit_devices/synchrotron/db_files/DCCT.db"
-    ioc_name: str = "BL03S-SR-DI-DCCT-01"
+    db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/DCCT.db")
+    ioc_name: str = "SR-DI-DCCT-01"
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
             device=SynchrotronCurrentDevice(
                 self.initial_current,
                 callback_period=self.callback_period,
             ),
             adapters=[
                 SynchrotronCurrentTCPAdapter(
                     TcpServer(self.host, self.port, self.format)
                 ),
-                SynchrotronCurrentEpicsAdapter(self.db_file, self.ioc_name),
+                SynchrotronCurrentEpicsAdapter(self.ioc_name, self.db_file),
             ],
         )
```

### Comparing `tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_machine.py` & `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_machine.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from dataclasses import dataclass
+import pathlib
+from typing import TypedDict
 
+import pydantic.v1.dataclasses
 from softioc import builder
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.epicsadapter import EpicsAdapter
 from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.adapter import Server
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 
 class SynchrotronMachineStatusDevice(Device):
     """Device to simulate the machine status records from the synchrotron.
 
     The signal is read via an epics adapter, and set using a tcp adapter.
     """
@@ -180,35 +181,35 @@
             self.device.get_user_countdown,
         )
         self.link_input_on_interrupt(
             builder.aIn("BEAMENERGY"), self.device.get_beam_energy
         )
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class SynchrotronMachineStatus(ComponentConfig):
     """Synchrotron Machine status component."""
 
     initial_mode: int = 4
     initial_countdown: float = 100000
     initial_energy: float = 3.0
     host: str = "localhost"
     port: int = 25565
     format: ByteFormat = ByteFormat(b"%b\r\n")
-    db_file: str = "src/tickit_devices/synchrotron/db_files/MSTAT.db"
-    ioc_name: str = "BL03S-CS-CS-MSTAT-01"
+    db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/MSTAT.db")
+    ioc_name: str = "CS-CS-MSTAT-01"
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
             device=SynchrotronMachineStatusDevice(
                 self.initial_mode,
                 self.initial_countdown,
                 self.initial_energy,
             ),
             adapters=[
                 SynchrotronMachineStatusTCPAdapter(
                     TcpServer(self.host, self.port, self.format)
                 ),
-                SynchrotronMachineStatusEpicsAdapter(self.db_file, self.ioc_name),
+                SynchrotronMachineStatusEpicsAdapter(self.ioc_name, self.db_file),
             ],
         )
```

### Comparing `tickit-devices-0.1.0/src/tickit_devices/synchrotron/synchrotron_topup.py` & `tickit-devices-0.2.0/src/tickit_devices/synchrotron/synchrotron_topup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-from dataclasses import dataclass
+import pathlib
+from typing import TypedDict
 
+import pydantic.v1.dataclasses
 from softioc import builder
 from tickit.adapters.composed import ComposedAdapter
 from tickit.adapters.epicsadapter import EpicsAdapter
 from tickit.adapters.interpreters.command import CommandInterpreter, RegexCommand
 from tickit.adapters.servers.tcp import TcpServer
 from tickit.core.adapter import Server
 from tickit.core.components.component import Component, ComponentConfig
 from tickit.core.components.device_simulation import DeviceSimulation
 from tickit.core.device import Device, DeviceUpdate
 from tickit.core.typedefs import SimTime
 from tickit.utils.byte_format import ByteFormat
-from tickit.utils.compat.typing_compat import TypedDict
 
 
 class SynchrotronTopUpDevice(Device):
     """Device to simulate the top up records from the synchrotron.
 
     The signal is read via an epics adapter, and set using a tcp adapter.
     """
@@ -201,35 +202,35 @@
         )
         self.link_input_on_interrupt(
             builder.aIn("ENDCOUNTDN"),
             self.device.get_end_countdown,
         )
 
 
-@dataclass
+@pydantic.v1.dataclasses.dataclass
 class SynchrotronTopUp(ComponentConfig):
     """Synchrotron top up status component."""
 
     initial_countdown: float = 600
     initial_end_countdown: float = 620
     callback_period: int = int(1e9)
     host: str = "localhost"
     port: int = 25565
     format: ByteFormat = ByteFormat(b"%b\r\n")
-    db_file: str = "src/tickit_devices/synchrotron/db_files/FILL.db"
-    ioc_name: str = "BL03S-SR-CS-FILL-01"
+    db_file: str = str(pathlib.Path(__file__).parent.absolute() / "db_files/FILL.db")
+    ioc_name: str = "SR-CS-FILL-01"
 
     def __call__(self) -> Component:  # noqa: D102
         return DeviceSimulation(
             name=self.name,
             device=SynchrotronTopUpDevice(
                 self.initial_countdown,
                 self.initial_end_countdown,
                 callback_period=self.callback_period,
             ),
             adapters=[
                 SynchrotronTopUpTCPAdapter(
                     TcpServer(self.host, self.port, self.format)
                 ),
-                SynchrotronTopUpEpicsAdapter(self.db_file, self.ioc_name),
+                SynchrotronTopUpEpicsAdapter(self.ioc_name, self.db_file),
             ],
         )
```

### Comparing `tickit-devices-0.1.0/src/tickit_devices.egg-info/PKG-INFO` & `tickit-devices-0.2.0/src/tickit_devices.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tickit-devices
-Version: 0.1.0
+Version: 0.2.0
 Summary: Devices for tickit, an event-based device simulation framework
 Author-email: Abigail Emery <abigail.emery@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -204,18 +204,17 @@
            WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
            See the License for the specific language governing permissions and
            limitations under the License.
         
 Project-URL: GitHub, https://github.com/dls-controls/tickit-devices
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 tickit-devices
 ===============
 
@@ -227,14 +226,22 @@
 PyPI           ``pip install tickit-devices``
 Source code    https://github.com/dls-controls/tickit-devices
 Documentation  https://dls-controls.github.io/tickit-devices
 Releases       https://github.com/dls-controls/tickit-devices/releases
 ============== ==============================================================
 
 
+Safety Note
+------------------------------------
+These devices mimic real synchrotron devices and there is the potential for conflict with the real PVs if this is run on the same port as EPICS (5064).
+If using this simulation to test software, set your ``EPICS_CA_SERVER_PORT`` environment variable to something nonstandard, e.g. 5065 or greater, so that your 
+tests are not confused between these and the real PVs. The `S03 <https://gitlab.diamond.ac.uk/controls/python3/s03_utils>`_ startup scripts manage the setting of
+these ports automatically, so if you are using this as part of S03 you won't need to change anything. Do not run this simulation on a beamline controls machine!
+
+
 Adding devices to the S03 simulation
 ------------------------------------
 To add a device to s03, the config file required to run the tickit simulation should be present in ``s03_configs``.
 Only changes pushed to main will be built into the ``tickit-devices`` image that s03 pulls from. Once the 
 image has been built with the new device and config, follow the instructions `here <https://gitlab.diamond.ac.uk/controls/python3/s03_utils>`_
 to include it in S03.
 
@@ -247,15 +254,15 @@
     :target: https://github.com/dls-controls/tickit-devices/actions/workflows/docs.yml
     :alt: Docs CI
 
 .. |coverage| image:: https://codecov.io/gh/dls-controls/tickit-devices/branch/main/graph/badge.svg
     :target: https://codecov.io/gh/dls-controls/tickit-devices
     :alt: Test Coverage
 
-.. |pypi_version| image:: https://img.shields.io/pypi/v/python3-pip-skeleton.svg
+.. |pypi_version| image:: https://img.shields.io/pypi/v/tickit-devices.svg
     :target: https://pypi.org/project/tickit-devices
     :alt: Latest PyPI version
 
 .. |license| image:: https://img.shields.io/badge/License-Apache%202.0-blue.svg
     :target: https://opensource.org/licenses/Apache-2.0
     :alt: Apache License
```

### Comparing `tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_current.py` & `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_current.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_machine.py` & `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_machine.py`

 * *Files identical despite different names*

### Comparing `tickit-devices-0.1.0/tests/synchrotron/test_synchrotron_topup.py` & `tickit-devices-0.2.0/tests/synchrotron/test_synchrotron_topup.py`

 * *Files identical despite different names*

