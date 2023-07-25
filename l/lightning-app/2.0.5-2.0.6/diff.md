# Comparing `tmp/lightning-app-2.0.5.tar.gz` & `tmp/lightning-app-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightning-app-2.0.5.tar", last modified: Mon Jul 10 16:10:51 2023, max compression
+gzip compressed data, was "lightning-app-2.0.6.tar", last modified: Mon Jul 24 21:37:48 2023, max compression
```

## Comparing `lightning-app-2.0.5.tar` & `lightning-app-2.0.6.tar`

### file list

```diff
@@ -1,366 +1,366 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/.actions/
--rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-10 16:10:36.000000 lightning-app-2.0.5/.actions/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-10 16:10:36.000000 lightning-app-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 16:10:51.591985 lightning-app-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-10 16:10:36.000000 lightning-app-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-10 16:10:36.000000 lightning-app-2.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.535984 lightning-app-2.0.5/requirements/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/requirements/app/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/cloud.txt
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/components.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-10 16:10:36.000000 lightning-app-2.0.5/requirements/app/ui.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:10:51.591985 lightning-app-2.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-10 16:10:36.000000 lightning-app-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.543984 lightning-app-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app/
--rw-r--r--   0 runner    (1001) docker     (123)    34568 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app/api/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/api/request_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.539984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.551984 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_clusters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_install.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_pl_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_react_ui_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/cmd_ssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/cd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/cp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/ls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/pwd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/commands/rm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.539984 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/placeholdername/component.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/connect/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/connect/maverick.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.555984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/.lightningignore
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/state.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/test_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.559984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/example_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
--rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/yarn.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.563984 lightning-app-2.0.5/src/lightning_app/components/database/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     9161 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/database/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/multi_node/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/fabric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/pytorch_spawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/multi_node/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/python/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/popen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/python/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/serve/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/auto_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-10 16:10:48.000000 lightning-app-2.0.5/src/lightning_app/components/serve/catimage.png
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/cold_start_proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/gradio_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/python_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/components/serve/types/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/serve/types/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/components/training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.567984 lightning-app-2.0.5/src/lightning_app/core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/flow.py
--rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/core/work.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/just_py/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/frontend/panel/
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_comm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_watcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_serve_render_fn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/stream_lit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/streamlit_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/frontend/web.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/perf/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/perf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/perf/pdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/plugin/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.571984 lightning-app-2.0.5/src/lightning_app/runners/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/backends/mp_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    47270 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/multiprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/runners/runtime_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/source_code/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/copytree.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/tar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/source_code/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/copier.py
--rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/storage/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/structures/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/structures/list.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/testing/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/ui/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.575984 lightning-app-2.0.5/src/lightning_app/ui/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.579985 lightning-app-2.0.5/src/lightning_app/ui/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css.map
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.579985 lightning-app-2.0.5/src/lightning_app/ui/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js
--rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.map
--rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/lightningState.js
--rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/manifest.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.583984 lightning-app-2.0.5/src/lightning_app/ui/static/media/
--rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
--rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
--rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
--rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
--rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.5/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
--rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.5/src/lightning_app/ui/static/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/app_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cli_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/cluster_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/clusters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/commands/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/data_structures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/dependency_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/introspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/load_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/log_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/logs_socket_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/name_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/openapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.591985 lightning-app-2.0.5/src/lightning_app/utilities/packaging/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/build_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/cloud_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/packaging/tarfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/port.py
--rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/safe_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-10 16:10:50.000000 lightning-app-2.0.5/src/lightning_app/utilities/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/lightning_app/version.info
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:10:51.547984 lightning-app-2.0.5/src/lightning_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 16:10:51.000000 lightning-app-2.0.5/src/lightning_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 16:10:36.000000 lightning-app-2.0.5/src/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.663018 lightning-app-2.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.631018 lightning-app-2.0.6/.actions/
+-rw-r--r--   0 runner    (1001) docker     (123)    19105 2023-07-24 21:37:36.000000 lightning-app-2.0.6/.actions/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-07-24 21:37:36.000000 lightning-app-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-24 21:37:48.663018 lightning-app-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    22065 2023-07-24 21:37:36.000000 lightning-app-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10138 2023-07-24 21:37:36.000000 lightning-app-2.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.627018 lightning-app-2.0.6/requirements/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.631018 lightning-app-2.0.6/requirements/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/cloud.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/components.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-24 21:37:36.000000 lightning-app-2.0.6/requirements/app/ui.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:37:48.663018 lightning-app-2.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8000 2023-07-24 21:37:36.000000 lightning-app-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.631018 lightning-app-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/
+-rw-r--r--   0 runner    (1001) docker     (123)    34738 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1974 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/api/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/api/request_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.627018 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_a/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_a/component_a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_b/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/placeholdername/components/component_b/component_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16481 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_clusters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5329 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21516 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_pl_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4348 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_react_ui_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/cmd_ssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12649 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/cp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4289 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/ls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/pwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/commands/rm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/component-template/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.627018 lightning-app-2.0.6/src/lightning_app/cli/component-template/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/component-template/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/component-template/placeholdername/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/placeholdername/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/placeholdername/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/component-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/component-template/tests/test_placeholdername_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14386 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/connect/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/connect/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/connect/maverick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20481 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/lightning_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8949 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/.lightningignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12991 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/script_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/script_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.639018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/lightning-colors.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/reportWebVitals.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/example_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/App.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/main.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/vite-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/tsconfig.node.json
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/vite.config.ts
+-rw-r--r--   0 runner    (1001) docker     (123)    55291 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.643018 lightning-app-2.0.6/src/lightning_app/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/components/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/database/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/database/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9322 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/database/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/components/multi_node/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/multi_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/multi_node/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/multi_node/fabric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/multi_node/pytorch_spawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/multi_node/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/components/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/python/popen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/python/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/components/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30440 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/auto_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20105 2023-07-24 21:37:46.000000 lightning-app-2.0.6/src/lightning_app/components/serve/catimage.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/cold_start_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/gradio_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/python_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5939 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/components/serve/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/types/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/serve/types/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/components/training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19330 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29679 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32847 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/flow.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18662 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31224 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/core/work.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.647018 lightning-app-2.0.6/src/lightning_app/frontend/just_py/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/just_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/just_py/just_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/just_py/just_py_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/frontend/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/panel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3287 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/panel/app_state_comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/panel/app_state_watcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/panel/panel_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/panel/panel_serve_render_fn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/stream_lit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/streamlit_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/frontend/web.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/perf/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/perf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/perf/pdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/plugin/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/plugin/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/runners/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/backends/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/backends/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5318 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/backends/mp_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47270 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/multiprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/runners/runtime_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/source_code/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6852 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6075 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3889 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/source_code/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/copier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6070 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18328 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10970 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/storage/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/structures/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/structures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/structures/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/structures/list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/testing/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/testing/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19756 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app/testing/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.651018 lightning-app-2.0.6/src/lightning_app/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.655018 lightning-app-2.0.6/src/lightning_app/ui/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.655018 lightning-app-2.0.6/src/lightning_app/ui/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/css/main.bb0f092c.css
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/css/main.bb0f092c.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2022-12-09 18:23:41.000000 lightning-app-2.0.6/src/lightning_app/ui/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.655018 lightning-app-2.0.6/src/lightning_app/ui/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/js/787.418637a8.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10281 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)   349883 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  1343802 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js.map
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2022-12-09 18:23:41.000000 lightning-app-2.0.6/src/lightning_app/ui/static/lightningState.js
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2022-12-09 18:23:41.000000 lightning-app-2.0.6/src/lightning_app/ui/static/manifest.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.655018 lightning-app-2.0.6/src/lightning_app/ui/static/media/
+-rw-r--r--   0 runner    (1001) docker     (123)    21692 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    29124 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    29800 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    22408 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    21108 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    28356 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/error.11892047d0183a4723b91dc0fb98cb95.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/success.5edae4c5b171e2c1c5a3c54273c47ba8.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-09 18:23:58.000000 lightning-app-2.0.6/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2022-12-09 18:23:41.000000 lightning-app-2.0.6/src/lightning_app/ui/static/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.659018 lightning-app-2.0.6/src/lightning_app/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/app_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20621 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/app_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/app_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/app_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/cli_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2498 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4752 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/cluster_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/clusters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.659018 lightning-app-2.0.6/src/lightning_app/utilities/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11195 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/data_structures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/dependency_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11480 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/introspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/load_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/log_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7928 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/logs_socket_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60255 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/name_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10417 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/openapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.663018 lightning-app-2.0.6/src/lightning_app/utilities/packaging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7631 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/build_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7516 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/cloud_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/packaging/tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30277 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4635 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/safe_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12598 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-24 21:37:47.000000 lightning-app-2.0.6/src/lightning_app/utilities/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/lightning_app/version.info
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 21:37:48.635018 lightning-app-2.0.6/src/lightning_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11136 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-24 21:37:48.000000 lightning-app-2.0.6/src/lightning_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-24 21:37:36.000000 lightning-app-2.0.6/src/version.info
```

### Comparing `lightning-app-2.0.5/.actions/assistant.py` & `lightning-app-2.0.6/.actions/assistant.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/LICENSE` & `lightning-app-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/PKG-INFO` & `lightning-app-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.5
+Version: 2.0.6
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.5 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.6 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
```

### Comparing `lightning-app-2.0.5/README.md` & `lightning-app-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/pyproject.toml` & `lightning-app-2.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/requirements/app/base.txt` & `lightning-app-2.0.6/requirements/app/base.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 lightning-cloud >=0.5.37
 packaging
 typing-extensions >=4.0.0, <=4.4.0
-deepdiff >=5.7.0, <6.3.1
+deepdiff >=5.7.0, <6.3.2
 starsessions >=1.2.1, <2.0 # strict
 fsspec >=2022.5.0, <=2023.6.0
 croniter >=1.3.0, <1.5.0  # strict; TODO: for now until we find something more robust.
 traitlets >=5.3.0, <5.10.0
 arrow >=1.2.0, <1.2.4
 lightning-utilities >=0.7.0, <0.10.0
 beautifulsoup4 >=4.8.0, <4.12.3
@@ -13,15 +13,15 @@
 psutil <5.9.5
 click <=8.1.3
 python-multipart>=0.0.5, <=0.0.6
 backoff >=2.2.1, <2.3.0
 
 fastapi >=0.92.0, <0.100.0
 starlette  # https://fastapi.tiangolo.com/deployment/versions/#about-starlette
-pydantic >=1.7.4, <2.0.0  # strict # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
+pydantic >=1.7.4, <2.1.0  # strict # https://fastapi.tiangolo.com/deployment/versions/#about-pydantic
 
 dateutils <=0.6.12
 Jinja2 <=3.1.2
 PyYAML <=6.0
 requests <2.31.1
 rich >=12.3.0, <=13.4.2
 urllib3 <=2.0.2
```

### Comparing `lightning-app-2.0.5/setup.py` & `lightning-app-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/CHANGELOG.md` & `lightning-app-2.0.6/src/lightning_app/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/).
 
 
+## [2.0.6] - 2023-07-20
+
+#### Fixed
+
+- Fixed handling a `None` request in the file orchestration queue ([#18111](https://github.com/Lightning-AI/lightning/pull/18111))
+
+
 ## [2.0.5] - 2023-07-07
 
 ### Added
 
 - plugin: store source app ([#17892](https://github.com/Lightning-AI/lightning/pull/17892))
 - added colocation identifier ([#16796](https://github.com/Lightning-AI/lightning/pull/16796))
 - Added exponential backoff to HTTPQueue put ([#18013](https://github.com/Lightning-AI/lightning/pull/18013))
```

### Comparing `lightning-app-2.0.5/src/lightning_app/README.md` & `lightning-app-2.0.6/src/lightning_app/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/__about__.py` & `lightning-app-2.0.6/src/lightning_app/__about__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/__init__.py` & `lightning-app-2.0.6/src/lightning_app/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/__setup__.py` & `lightning-app-2.0.6/src/lightning_app/__setup__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/api/http_methods.py` & `lightning-app-2.0.6/src/lightning_app/api/http_methods.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/api/request_types.py` & `lightning-app-2.0.6/src/lightning_app/api/request_types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/app-template/.gitignore` & `lightning-app-2.0.6/src/lightning_app/cli/app-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/app-template/LICENSE` & `lightning-app-2.0.6/src/lightning_app/cli/app-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/app-template/README.md` & `lightning-app-2.0.6/src/lightning_app/cli/app-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py` & `lightning-app-2.0.6/src/lightning_app/cli/app-template/tests/test_placeholdername_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_apps.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_apps.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_clusters.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_init.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_install.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_install.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_pl_init.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_pl_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_react_ui_init.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_react_ui_init.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/cmd_ssh_keys.py` & `lightning-app-2.0.6/src/lightning_app/cli/cmd_ssh_keys.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/app_commands.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/cd.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/cd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/cp.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/cp.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/logs.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/ls.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/ls.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/pwd.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/pwd.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/commands/rm.py` & `lightning-app-2.0.6/src/lightning_app/cli/commands/rm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml` & `lightning-app-2.0.6/src/lightning_app/cli/component-template/.github/workflows/ci-testing.yml`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/component-template/.gitignore` & `lightning-app-2.0.6/src/lightning_app/cli/component-template/.gitignore`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/component-template/LICENSE` & `lightning-app-2.0.6/src/lightning_app/cli/component-template/LICENSE`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/component-template/README.md` & `lightning-app-2.0.6/src/lightning_app/cli/component-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/connect/app.py` & `lightning-app-2.0.6/src/lightning_app/cli/connect/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/connect/data.py` & `lightning-app-2.0.6/src/lightning_app/cli/connect/data.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/connect/maverick.py` & `lightning-app-2.0.6/src/lightning_app/cli/connect/maverick.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/core.py` & `lightning-app-2.0.6/src/lightning_app/cli/core.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli.py` & `lightning-app-2.0.6/src/lightning_app/cli/lightning_cli.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_create.py` & `lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_create.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_delete.py` & `lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_delete.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/lightning_cli_list.py` & `lightning-app-2.0.6/src/lightning_app/cli/lightning_cli_list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/app.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/callbacks.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/tensorboard.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/logger/weights_and_biases.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/components/script_runner/script_runner.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/core/state.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/core/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/setup.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/setup.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/tests/core/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/.prettierrc` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/.prettierrc`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/craco.config.js` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/craco.config.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/package.json` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/public/index.html` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/public/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/App.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/EnvironmentConfigurator.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ErrorPanel.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ExecutionSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/HyperparameterSummary.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/Launcher.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBar.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/ProgressBarGroup.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/components/Timer.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/index.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/index.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/pl-app-template/ui/tsconfig.json` & `lightning-app-2.0.6/src/lightning_app/cli/pl-app-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/README.md` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/README.md`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/example_app.py` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/example_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/package.json` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/package.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/App.tsx` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/App.tsx`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/favicon.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/hooks/useLightningState.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/src/types/lightning.ts`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/tsconfig.json` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/tsconfig.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/cli/react-ui-template/ui/yarn.lock` & `lightning-app-2.0.6/src/lightning_app/cli/react-ui-template/ui/yarn.lock`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/__init__.py` & `lightning-app-2.0.6/src/lightning_app/components/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/database/client.py` & `lightning-app-2.0.6/src/lightning_app/components/database/client.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/database/server.py` & `lightning-app-2.0.6/src/lightning_app/components/database/server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/database/utilities.py` & `lightning-app-2.0.6/src/lightning_app/components/database/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,21 @@
 import functools
 import json
 import pathlib
 from typing import Any, Dict, Generic, List, Type, TypeVar
 
 from fastapi import Response, status
 from fastapi.encoders import jsonable_encoder
+from lightning_utilities.core.imports import RequirementCache
 from pydantic import BaseModel, parse_obj_as
-from pydantic.main import ModelMetaclass
+
+if RequirementCache("pydantic>=2.0.0"):
+    from pydantic.v1.main import ModelMetaclass
+else:
+    from pydantic.main import ModelMetaclass
 
 from lightning_app.utilities.app_helpers import Logger
 from lightning_app.utilities.imports import _is_sqlmodel_available
 
 if _is_sqlmodel_available():
     from sqlalchemy.inspection import inspect as sqlalchemy_inspect
     from sqlmodel import JSON, select, Session, SQLModel, TypeDecorator
```

### Comparing `lightning-app-2.0.5/src/lightning_app/components/multi_node/base.py` & `lightning-app-2.0.6/src/lightning_app/components/multi_node/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/multi_node/fabric.py` & `lightning-app-2.0.6/src/lightning_app/components/multi_node/fabric.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/multi_node/pytorch_spawn.py` & `lightning-app-2.0.6/src/lightning_app/components/multi_node/pytorch_spawn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/multi_node/trainer.py` & `lightning-app-2.0.6/src/lightning_app/components/multi_node/trainer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/python/popen.py` & `lightning-app-2.0.6/src/lightning_app/components/python/popen.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/python/tracer.py` & `lightning-app-2.0.6/src/lightning_app/components/python/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/__init__.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/auto_scaler.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/auto_scaler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/catimage.png` & `lightning-app-2.0.6/src/lightning_app/components/serve/catimage.png`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/cold_start_proxy.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/cold_start_proxy.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/gradio_server.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/gradio_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/python_server.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/python_server.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/serve.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/serve.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/streamlit.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/streamlit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/types/image.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/types/image.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/serve/types/type.py` & `lightning-app-2.0.6/src/lightning_app/components/serve/types/type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/components/training.py` & `lightning-app-2.0.6/src/lightning_app/components/training.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/api.py` & `lightning-app-2.0.6/src/lightning_app/core/api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/app.py` & `lightning-app-2.0.6/src/lightning_app/core/app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/constants.py` & `lightning-app-2.0.6/src/lightning_app/core/constants.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/flow.py` & `lightning-app-2.0.6/src/lightning_app/core/flow.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/queues.py` & `lightning-app-2.0.6/src/lightning_app/core/queues.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/core/work.py` & `lightning-app-2.0.6/src/lightning_app/core/work.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/frontend.py` & `lightning-app-2.0.6/src/lightning_app/frontend/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py.py` & `lightning-app-2.0.6/src/lightning_app/frontend/just_py/just_py.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/just_py/just_py_base.py` & `lightning-app-2.0.6/src/lightning_app/frontend/just_py/just_py_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_comm.py` & `lightning-app-2.0.6/src/lightning_app/frontend/panel/app_state_comm.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/panel/app_state_watcher.py` & `lightning-app-2.0.6/src/lightning_app/frontend/panel/app_state_watcher.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_frontend.py` & `lightning-app-2.0.6/src/lightning_app/frontend/panel/panel_frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/panel/panel_serve_render_fn.py` & `lightning-app-2.0.6/src/lightning_app/frontend/panel/panel_serve_render_fn.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/stream_lit.py` & `lightning-app-2.0.6/src/lightning_app/frontend/stream_lit.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/streamlit_base.py` & `lightning-app-2.0.6/src/lightning_app/frontend/streamlit_base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/utils.py` & `lightning-app-2.0.6/src/lightning_app/frontend/utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/frontend/web.py` & `lightning-app-2.0.6/src/lightning_app/frontend/web.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/perf/pdb.py` & `lightning-app-2.0.6/src/lightning_app/perf/pdb.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/plugin/actions.py` & `lightning-app-2.0.6/src/lightning_app/plugin/actions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/plugin/plugin.py` & `lightning-app-2.0.6/src/lightning_app/plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/backends/__init__.py` & `lightning-app-2.0.6/src/lightning_app/runners/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/backends/backend.py` & `lightning-app-2.0.6/src/lightning_app/runners/backends/backend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/backends/cloud.py` & `lightning-app-2.0.6/src/lightning_app/runners/backends/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/backends/docker.py` & `lightning-app-2.0.6/src/lightning_app/runners/backends/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/backends/mp_process.py` & `lightning-app-2.0.6/src/lightning_app/runners/backends/mp_process.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/cloud.py` & `lightning-app-2.0.6/src/lightning_app/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/multiprocess.py` & `lightning-app-2.0.6/src/lightning_app/runners/multiprocess.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/runtime.py` & `lightning-app-2.0.6/src/lightning_app/runners/runtime.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/runners/runtime_type.py` & `lightning-app-2.0.6/src/lightning_app/runners/runtime_type.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/source_code/copytree.py` & `lightning-app-2.0.6/src/lightning_app/source_code/copytree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/source_code/hashing.py` & `lightning-app-2.0.6/src/lightning_app/source_code/hashing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/source_code/local.py` & `lightning-app-2.0.6/src/lightning_app/source_code/local.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/source_code/tar.py` & `lightning-app-2.0.6/src/lightning_app/source_code/tar.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/source_code/uploader.py` & `lightning-app-2.0.6/src/lightning_app/source_code/uploader.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/copier.py` & `lightning-app-2.0.6/src/lightning_app/storage/copier.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/drive.py` & `lightning-app-2.0.6/src/lightning_app/storage/drive.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/filesystem.py` & `lightning-app-2.0.6/src/lightning_app/storage/filesystem.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/mount.py` & `lightning-app-2.0.6/src/lightning_app/storage/mount.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/orchestrator.py` & `lightning-app-2.0.6/src/lightning_app/storage/orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,19 @@
     def run_once(self, work_name: str) -> None:
         if work_name not in self.waiting_for_response:
             # check if there is a new request from this work for a file transfer
             # there can only be one pending request per work
             request_queue = self.request_queues[work_name]
             try:
                 request: _PathRequest = request_queue.get(timeout=0)  # this should not block
+                # This should not happen under normal conditions, but it has occurred.
+                # For now we are tolerant with respect to requests being None in the queue
+                # and just move on.
+                if request is None:
+                    raise Empty
             except Empty:
                 pass
             else:
                 request.destination = work_name
                 source_work = self.app.get_component_by_name(request.source)
                 maybe_artifact_path = str(_path_to_work_artifact(request.path, source_work))
```

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/path.py` & `lightning-app-2.0.6/src/lightning_app/storage/path.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/payload.py` & `lightning-app-2.0.6/src/lightning_app/storage/payload.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/storage/requests.py` & `lightning-app-2.0.6/src/lightning_app/storage/requests.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/structures/dict.py` & `lightning-app-2.0.6/src/lightning_app/structures/dict.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/structures/list.py` & `lightning-app-2.0.6/src/lightning_app/structures/list.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/testing/config.py` & `lightning-app-2.0.6/src/lightning_app/testing/config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/testing/helpers.py` & `lightning-app-2.0.6/src/lightning_app/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/testing/testing.py` & `lightning-app-2.0.6/src/lightning_app/testing/testing.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/asset-manifest.json` & `lightning-app-2.0.6/src/lightning_app/ui/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/index.html` & `lightning-app-2.0.6/src/lightning_app/ui/index.html`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css` & `lightning-app-2.0.6/src/lightning_app/ui/static/css/main.bb0f092c.css`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/css/main.bb0f092c.css.map` & `lightning-app-2.0.6/src/lightning_app/ui/static/css/main.bb0f092c.css.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/favicon.ico` & `lightning-app-2.0.6/src/lightning_app/ui/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js` & `lightning-app-2.0.6/src/lightning_app/ui/static/js/787.418637a8.chunk.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map` & `lightning-app-2.0.6/src/lightning_app/ui/static/js/787.418637a8.chunk.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js` & `lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt` & `lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/js/main.2b242b99.js.map` & `lightning-app-2.0.6/src/lightning_app/ui/static/js/main.2b242b99.js.map`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/lightningState.js` & `lightning-app-2.0.6/src/lightning_app/ui/static/lightningState.js`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Light.30446c15a21bf8a994e8.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Light.47cf3e33cb6bb1496c95.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Regular.7a3b475525ed92dc7816.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Regular.8afa44ac39706d62b62b.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Semibold.80655a0e8b4bb5f30545.woff2`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/UCity-Semibold.bb7aab96e378ebd6a651.woff`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/lightning-logo-with-text.b964c8fbf221c97eb8ce52bb6e3a30d6.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg` & `lightning-app-2.0.6/src/lightning_app/ui/static/media/warning.5c542673e84e77ceb6a230bfea7f7263.svg`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/app_commands.py` & `lightning-app-2.0.6/src/lightning_app/utilities/app_commands.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/app_helpers.py` & `lightning-app-2.0.6/src/lightning_app/utilities/app_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/app_logs.py` & `lightning-app-2.0.6/src/lightning_app/utilities/app_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/app_status.py` & `lightning-app-2.0.6/src/lightning_app/utilities/app_status.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/auth.py` & `lightning-app-2.0.6/src/lightning_app/utilities/auth.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/cli_helpers.py` & `lightning-app-2.0.6/src/lightning_app/utilities/cli_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/cloud.py` & `lightning-app-2.0.6/src/lightning_app/utilities/cloud.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/cluster_logs.py` & `lightning-app-2.0.6/src/lightning_app/utilities/cluster_logs.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/clusters.py` & `lightning-app-2.0.6/src/lightning_app/utilities/clusters.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/commands/base.py` & `lightning-app-2.0.6/src/lightning_app/utilities/commands/base.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/component.py` & `lightning-app-2.0.6/src/lightning_app/utilities/component.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/data_structures.py` & `lightning-app-2.0.6/src/lightning_app/utilities/data_structures.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/dependency_caching.py` & `lightning-app-2.0.6/src/lightning_app/utilities/dependency_caching.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/enum.py` & `lightning-app-2.0.6/src/lightning_app/utilities/enum.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/exceptions.py` & `lightning-app-2.0.6/src/lightning_app/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/frontend.py` & `lightning-app-2.0.6/src/lightning_app/utilities/frontend.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/git.py` & `lightning-app-2.0.6/src/lightning_app/utilities/git.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/imports.py` & `lightning-app-2.0.6/src/lightning_app/utilities/imports.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/introspection.py` & `lightning-app-2.0.6/src/lightning_app/utilities/introspection.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/layout.py` & `lightning-app-2.0.6/src/lightning_app/utilities/layout.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/load_app.py` & `lightning-app-2.0.6/src/lightning_app/utilities/load_app.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/log.py` & `lightning-app-2.0.6/src/lightning_app/utilities/log.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/log_helpers.py` & `lightning-app-2.0.6/src/lightning_app/utilities/log_helpers.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/login.py` & `lightning-app-2.0.6/src/lightning_app/utilities/login.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/logs_socket_api.py` & `lightning-app-2.0.6/src/lightning_app/utilities/logs_socket_api.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/name_generator.py` & `lightning-app-2.0.6/src/lightning_app/utilities/name_generator.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/network.py` & `lightning-app-2.0.6/src/lightning_app/utilities/network.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/openapi.py` & `lightning-app-2.0.6/src/lightning_app/utilities/openapi.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/app_config.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/app_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/build_config.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/build_config.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/cloud_compute.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/cloud_compute.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/docker.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/docker.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/lightning_utils.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/lightning_utils.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/packaging/tarfile.py` & `lightning-app-2.0.6/src/lightning_app/utilities/packaging/tarfile.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/port.py` & `lightning-app-2.0.6/src/lightning_app/utilities/port.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/proxies.py` & `lightning-app-2.0.6/src/lightning_app/utilities/proxies.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/redis.py` & `lightning-app-2.0.6/src/lightning_app/utilities/redis.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/safe_pickle.py` & `lightning-app-2.0.6/src/lightning_app/utilities/safe_pickle.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/scheduler.py` & `lightning-app-2.0.6/src/lightning_app/utilities/scheduler.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/secrets.py` & `lightning-app-2.0.6/src/lightning_app/utilities/secrets.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/state.py` & `lightning-app-2.0.6/src/lightning_app/utilities/state.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/tracer.py` & `lightning-app-2.0.6/src/lightning_app/utilities/tracer.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/tree.py` & `lightning-app-2.0.6/src/lightning_app/utilities/tree.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/types.py` & `lightning-app-2.0.6/src/lightning_app/utilities/types.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app/utilities/warnings.py` & `lightning-app-2.0.6/src/lightning_app/utilities/warnings.py`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app.egg-info/PKG-INFO` & `lightning-app-2.0.6/src/lightning_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightning-app
-Version: 2.0.5
+Version: 2.0.6
 Summary: Use Lightning Apps to build everything from production-ready, multi-cloud ML systems to simple research demos.
 Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al.
 Author-email: name@pytorchlightning.ai
 License: Apache-2.0
 Download-URL: https://github.com/Lightning-AI/lightning
 Project-URL: Bug Tracker, https://github.com/Lightning-AI/lightning/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lightning-app Version: 2.0.5 Summary: Use Lightning
+Metadata-Version: 2.1 Name: lightning-app Version: 2.0.6 Summary: Use Lightning
 Apps to build everything from production-ready, multi-cloud ML systems to
 simple research demos. Home-page: https://github.com/Lightning-AI/lightning
 Author: Lightning-AI et al. Author-email: name@pytorchlightning.ai License:
 Apache-2.0 Download-URL: https://github.com/Lightning-AI/lightning Project-URL:
 Bug Tracker, https://github.com/Lightning-AI/lightning/issues Project-URL:
 Documentation, https://lightning.ai/lightning-docs Project-URL: Source Code,
 https://github.com/Lightning-AI/lightning Keywords: deep learning,pytorch,AI
```

### Comparing `lightning-app-2.0.5/src/lightning_app.egg-info/SOURCES.txt` & `lightning-app-2.0.6/src/lightning_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightning-app-2.0.5/src/lightning_app.egg-info/requires.txt` & `lightning-app-2.0.6/src/lightning_app.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 inquirer<4.0,>=2.10.0
 psutil<6.0
 click<9.0
 python-multipart<1.0,>=0.0.5
 backoff<3.0,>=2.2.1
 fastapi<1.0,>=0.92.0
 starlette
-pydantic<2.0.0,>=1.7.4
+pydantic<2.1.0,>=1.7.4
 dateutils<1.0
 Jinja2<4.0
 PyYAML<7.0
 requests<3.0
 rich<14.0,>=12.3.0
 urllib3<3.0
 uvicorn<1.0
```

