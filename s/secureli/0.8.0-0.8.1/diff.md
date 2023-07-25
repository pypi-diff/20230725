# Comparing `tmp/secureli-0.8.0.tar.gz` & `tmp/secureli-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secureli-0.8.0.tar", max compression
+gzip compressed data, was "secureli-0.8.1.tar", max compression
```

## Comparing `secureli-0.8.0.tar` & `secureli-0.8.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11343 2023-07-18 20:02:34.146263 secureli-0.8.0/LICENSE
--rw-r--r--   0        0        0    11614 2023-07-18 20:02:34.146263 secureli-0.8.0/README.md
--rw-r--r--   0        0        0     2070 2023-07-18 20:02:34.150263 secureli-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/__init__.py
--rw-r--r--   0        0        0     3919 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/echo.py
--rw-r--r--   0        0        0      550 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/lexer_guesser.py
--rw-r--r--   0        0        0     6906 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/abstractions/pre_commit.py
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/__init__.py
--rw-r--r--   0        0        0    11784 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/action.py
--rw-r--r--   0        0        0      761 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/build.py
--rw-r--r--   0        0        0     1160 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/initializer.py
--rw-r--r--   0        0        0    10628 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/scan.py
--rw-r--r--   0        0        0      791 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/setup.py
--rw-r--r--   0        0        0     2087 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/actions/update.py
--rw-r--r--   0        0        0     6450 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/container.py
--rw-r--r--   0        0        0     2807 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/main.py
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/__init__.py
--rw-r--r--   0        0        0     3685 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/repo_files.py
--rw-r--r--   0        0        0     3632 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/secureli_config.py
--rw-r--r--   0        0        0     3926 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/repositories/settings.py
--rw-r--r--   0        0        0       59 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/__init__.py
--rw-r--r--   0        0        0      791 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/base-pre-commit.yaml
--rw-r--r--   0        0        0     4883 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/build.txt
--rw-r--r--   0        0        0       93 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/configs/javascript.config.yaml
--rw-r--r--   0        0        0      161 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/configs/typescript.config.yaml
--rw-r--r--   0        0        0      659 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/csharp-pre-commit.yaml
--rw-r--r--   0        0        0      461 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/epilog.md
--rw-r--r--   0        0        0      115 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/go-pre-commit.yaml
--rw-r--r--   0        0        0      130 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/java-pre-commit.yaml
--rw-r--r--   0        0        0      618 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/javascript-pre-commit.yaml
--rw-r--r--   0        0        0      367 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/python-pre-commit.yaml
--rw-r--r--   0        0        0      356 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/secrets_detecting_repos.yaml
--rw-r--r--   0        0        0      232 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/swift-pre-commit.yaml
--rw-r--r--   0        0        0      228 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/terraform-pre-commit.yaml
--rw-r--r--   0        0        0      714 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/files/typescript-pre-commit.yaml
--rw-r--r--   0        0        0      817 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/read_resource.py
--rw-r--r--   0        0        0     1325 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/resources/slugify.py
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/git_ignore.py
--rw-r--r--   0        0        0     3505 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_analyzer.py
--rw-r--r--   0        0        0    12318 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_config.py
--rw-r--r--   0        0        0    18724 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/language_support.py
--rw-r--r--   0        0        0     4470 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/logging.py
--rw-r--r--   0        0        0     6374 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/scanner.py
--rw-r--r--   0        0        0     1180 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/secureli_ignore.py
--rw-r--r--   0        0        0     3048 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/services/updater.py
--rw-r--r--   0        0        0     1482 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/settings.py
--rw-r--r--   0        0        0        0 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/__init__.py
--rw-r--r--   0        0        0     1080 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/git_meta.py
--rw-r--r--   0        0        0      254 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/hash.py
--rw-r--r--   0        0        0     1372 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/patterns.py
--rw-r--r--   0        0        0      198 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/secureli_meta.py
--rw-r--r--   0        0        0     1028 2023-07-18 20:02:34.150263 secureli-0.8.0/secureli/utilities/usage_stats.py
--rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 secureli-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2023-07-25 20:44:51.528949 secureli-0.8.1/LICENSE
+-rw-r--r--   0        0        0    12497 2023-07-25 20:44:51.528949 secureli-0.8.1/README.md
+-rw-r--r--   0        0        0     2068 2023-07-25 20:44:51.528949 secureli-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/abstractions/__init__.py
+-rw-r--r--   0        0        0     3919 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/abstractions/echo.py
+-rw-r--r--   0        0        0      550 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/abstractions/lexer_guesser.py
+-rw-r--r--   0        0        0     6906 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/abstractions/pre_commit.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/__init__.py
+-rw-r--r--   0        0        0    11784 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/action.py
+-rw-r--r--   0        0        0      761 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/build.py
+-rw-r--r--   0        0        0     1160 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/initializer.py
+-rw-r--r--   0        0        0    10628 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/scan.py
+-rw-r--r--   0        0        0      791 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/setup.py
+-rw-r--r--   0        0        0     2087 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/actions/update.py
+-rw-r--r--   0        0        0     6450 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/container.py
+-rw-r--r--   0        0        0     2807 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/main.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/repositories/__init__.py
+-rw-r--r--   0        0        0     3685 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/repositories/repo_files.py
+-rw-r--r--   0        0        0     3632 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/repositories/secureli_config.py
+-rw-r--r--   0        0        0     3926 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/repositories/settings.py
+-rw-r--r--   0        0        0       59 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/__init__.py
+-rw-r--r--   0        0        0      791 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/base-pre-commit.yaml
+-rw-r--r--   0        0        0     4883 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/build.txt
+-rw-r--r--   0        0        0       93 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/configs/javascript.config.yaml
+-rw-r--r--   0        0        0      161 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/configs/typescript.config.yaml
+-rw-r--r--   0        0        0      659 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/csharp-pre-commit.yaml
+-rw-r--r--   0        0        0      461 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/epilog.md
+-rw-r--r--   0        0        0      115 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/go-pre-commit.yaml
+-rw-r--r--   0        0        0      130 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/java-pre-commit.yaml
+-rw-r--r--   0        0        0      618 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/javascript-pre-commit.yaml
+-rw-r--r--   0        0        0      367 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/python-pre-commit.yaml
+-rw-r--r--   0        0        0      356 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/secrets_detecting_repos.yaml
+-rw-r--r--   0        0        0      232 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/swift-pre-commit.yaml
+-rw-r--r--   0        0        0      228 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/terraform-pre-commit.yaml
+-rw-r--r--   0        0        0      714 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/files/typescript-pre-commit.yaml
+-rw-r--r--   0        0        0      817 2023-07-25 20:44:51.528949 secureli-0.8.1/secureli/resources/read_resource.py
+-rw-r--r--   0        0        0     1325 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/resources/slugify.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/__init__.py
+-rw-r--r--   0        0        0     3646 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/git_ignore.py
+-rw-r--r--   0        0        0     3505 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/language_analyzer.py
+-rw-r--r--   0        0        0    12318 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/language_config.py
+-rw-r--r--   0        0        0    18724 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/language_support.py
+-rw-r--r--   0        0        0     4614 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/logging.py
+-rw-r--r--   0        0        0     6374 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/scanner.py
+-rw-r--r--   0        0        0     1180 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/secureli_ignore.py
+-rw-r--r--   0        0        0     3048 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/services/updater.py
+-rw-r--r--   0        0        0     1482 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/settings.py
+-rw-r--r--   0        0        0        0 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/__init__.py
+-rw-r--r--   0        0        0     1080 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/git_meta.py
+-rw-r--r--   0        0        0      254 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/hash.py
+-rw-r--r--   0        0        0     1372 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/patterns.py
+-rw-r--r--   0        0        0      198 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/secureli_meta.py
+-rw-r--r--   0        0        0     1028 2023-07-25 20:44:51.532949 secureli-0.8.1/secureli/utilities/usage_stats.py
+-rw-r--r--   0        0        0    13409 1970-01-01 00:00:00.000000 secureli-0.8.1/PKG-INFO
```

### Comparing `secureli-0.8.0/LICENSE` & `secureli-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/README.md` & `secureli-0.8.1/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -11,45 +11,47 @@
 - installs linters based on the code of your project to support security and coding best practices
 - configures all the hooks needed so you don’t have to
 
 SeCureLI isn’t a magic tool that makes things secure because you have it. It enables a lot of other tools that you could set up individually and helps you as a builder write better code.
 
 Looking to contribute? Read our [CONTRIBUTING.md](https://github.com/slalombuild/secureli/blob/main/CONTRIBUTING.md)
 
-# Installation and Usage
+# Installation
 
-## Secureli Installation via Homebrew
+## Homebrew
 
-Current the only packaging tool that is supported for Secureli is Homebrew. To install secureli via homebrew, issue the following commands
+To install seCureLI via homebrew, issue the following commands
 
 ```commandline
 brew tap slalombuild/secureli
 brew install secureli
 ```
 
-## Upgrading Secureli via Homebrew
+## pip (Package Installer for Python)
 
-To update secureli, you can use the standard homebrew update command to pull down the latest formula
+To install seCureLI via pip, issue the following commands
 
 ```commandline
-brew update
+pip install secureli
 ```
 
 # Usage
 
-Once installed you can see the latest documentation for SeCureLI by entering the following on a command prompt:
+## Help
+
+Once installed you can see the latest documentation for seCureLI by entering the following on a command prompt:
 
 ```python
 % secureli --help
 ```
 
 You will see a list of commands and descriptions of each. You can also pull up documentation for each command with the same pattern. For example:
 
 ```python
-(secureli-py3.9) tristan@Tristans-MacBook-Pro secureli % secureli init --help
+% secureli init --help
 
  Usage: secureli init [OPTIONS]
 
  Detect languages and initialize pre-commit hooks and linters for the project
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────╮
 │ --reset  -r        Disregard the installed configuration, if any, and treat as a new install   │
@@ -60,83 +62,120 @@
 
 When invoking these commands, you can combine the short versions into a single flag. For example, the following commands are equivalent:
 
 ```python
 % secureli init --reset --yes
 % secureli init -ry
 ```
+## Init
 
-# Tutorial to Use Observability Platform to Show Usage Statistics
+After seCureLI is installed, you can use it to configure your local git repository with a set of pre-commit hooks appropriate for your repo, based on the languages found in your repo's source code files.
 
-This tutorial uses New Relic as the sample observability platform. Other platforms may also work, but have not been tested.
-Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+All you need to do is run:
 
-## Steps
+```commandline
+% secureli init
+```
 
-- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
-- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
-- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
-- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
-- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+Running secureli init will allow secureli to detect the languages in your repo, install pre-commit, install all the appropriate pre-commit hooks for your local repo, and run a scan for secrets in your local repo.
+
+# Upgrade
+
+## Upgrading seCureLI via Homebrew
+
+If you installed seCureLI using Homebrew, you can use the standard homebrew update command to pull down the latest formula.
 
 ```commandline
-FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+brew update
+```
+## Upgrading via pip
+
+If you installed seCureLI using pip, you can use the following command to upgrade to the latest version of seCureLI.
+
+```commandline
+pip install --upgrade secureli
+```
+## Upgrading pre-commit hooks for repo
+
+In order to upgrade to the latest released version of each pre-commit hook configured for your repo, use the following command.
+
+```commandline
+secureli update --latest
 ```
 
 # Configuration
 
-SeCureLI is configurable via a .secureli.yaml file present in the consuming repository.
+SeCureLI is configurable via a .secureli.yaml file present in the root of your local repository.
+
+## .secureli.yaml
 
-## .secureli.yaml - top level
+### top level
 
 | Key                | Description                                                                                                                      |
 | ------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
 | `repo_files`       | Affects how SeCureLI will interpret the repository, both for language analysis and as it executes various linters.               |
 | `echo`             | Adjusts how SeCureLI will print information to the user.                                                                         |
 | `language_support` | Affects SeCureLI's language analysis and support phase.                                                                          |
 | `pre_commit`       | Enables various overrides and options for SeCureLI's configuration and usage of pre-commit, the underlying code analysis system. |
 
-## .secureli.yaml - repo_files
+### repo_files
 
 | Key                       | Description                                                                                                                                                                                                                                                             |
 | ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `max_file_size`           | A number in bytes. Files over this size will not be considered during language analysis, for speed purposes. Default: 100000                                                                                                                                            |
 | `ignored_file_extensions` | Which file extensions not to consider during language analysis.                                                                                                                                                                                                         |
 | `exclude_file_patterns`   | Which file patterns to ignore during language analysis and code analysis execution. Use a typical file pattern you might find in a .gitignore file, such as `*.py` or `tests/`. Certain patterns you will have to wrap in double-quotes for the entry to be valid YAML. |
 
-## .secureli.yaml - echo
+### echo
 
 | Key     | Description                                                                                                                                        |
 | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `level` | The log level to display to the user. Defaults to ERROR, which includes `error` and `print` messages, without including warnings or info messages. |
 
-## .secureli.yaml - pre_commit
+### pre_commit
 
 | Key                | Description                                                                                                                                                                                                                               |
 | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `repos`            | A set of template-based Pre-Commit Repos to configure with overrides, identified by URL. These override repo-configurations stored in the template, and attempting to modify a repo not configured into the template will have no effect. |
 | `suppressed_repos` | A set of template-based Pre-Commit Repo URLs to completely remove from the final configuration. These remove repo configurations stored in the template, removing a repo not stored in the template will be ignored.                      |
 
-## .secureli.yaml - pre_commit.repos
+### pre_commit.repos
 
 | Key                   | Description                                                                                                                                            |
 | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | `url`                 | The identifying URL of the repo being leveraged by pre-commit, within which one or more hooks can be leveraged.                                        |
 | `hooks`               | A set of hooks associated with the specified repository to override. See the next section for what we can configure there.                             |
 | `suppressed_hook_ids` | A set of hook IDs to remove from the repository as configured within the template. Hook IDs not present in the template configuration will be ignored. |
 
-## .secureli.yaml - pre_commit.repos.hooks
+### pre_commit.repos.hooks
 
 | Key                     | Description                                                                                                                                                                                                                                                                  |
 | ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `id`                    | The identifying string of the pre-commit hook to override.                                                                                                                                                                                                                   |
 | `arguments`             | A set of arguments to provide to the pre-commit hook identified by `id`. These arguments overwrite any existing arguments.                                                                                                                                                   |
 | `additional_args`       | A set of arguments to provide to the pre-commit hook identified by `id`. These arguments are appended after an existing arguments.                                                                                                                                           |
 | `exclude_file_patterns` | A set of file patterns to provide to pre-commit to ignore for the purposes of this hook. Use a typical file pattern you might find in a .gitignore file, such as `*.py` or `tests/`. Certain patterns you will have to wrap in double-quotes for the entry to be valid YAML. |
 
+## Using Observability Platform to Show Secret Detection Statistics
+
+SeCureLI can send secret detection events to an observability platform, such as New Relic.  Other platforms may also work, but have not been tested.
+Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+
+### Steps for New Relic
+
+- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
+- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
+- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
+- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
+- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+
+```commandline
+FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+```
+
 ## License
 
 Copyright 2023 Slalom, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `secureli-0.8.0/pyproject.toml` & `secureli-0.8.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secureli"
-version = "0.8.0"
+version = "0.8.1"
 description = "Secure Project Manager"
 authors = ["Caleb Tonn <caleb.tonn@slalom.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 
 [tool.poetry.scripts]
 secureli = "secureli.main:app"
@@ -18,15 +18,15 @@
 docker-build-homebrew = "docker build -t homebrew . -f Dockerfile_homebrew --no-cache --progress=plain"
 docker-build-pypi = "docker build -t pypi . -f Dockerfile_pypi --no-cache --progress=plain"
 init = ["install", "secureli_init"]
 secureli_init = "secureli init -y"
 install = "poetry install"
 lint = "black --check ."
 precommit = "pre-commit run -a"
-test = ["init", "lint", "coverage_run", "coverage_html"]
+test = ["init", "lint", "coverage_run", "coverage_report"]
 e2e = "bats tests/end-to-end/test.bats"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 typer = {version = ">=0.6.1,<0.10.0", extras = ["all"]}
 pygments = "^2.13.0"
 dependency-injector = {version = "^4.40.0", extras = ["yaml"]}
@@ -44,27 +44,25 @@
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 pytest-mock = "^3.10.0"
 coverage = ">=6.5,<8.0"
 black = ">=22.10,<24.0"
 identify = "^2.5.7"
 poethepoet = ">=0.16.4,<0.22.0"
-python-semantic-release = ">=7.33.1,<9.0.0"
+python-semantic-release = ">=8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
-version_toml = [
-    "pyproject.toml:tool.poetry.version"
-]
+version_toml = ["pyproject.toml:tool.poetry.version"]
 major_on_zero = true
 branch = "main"
 upload_to_PyPI = false
-upload_to_release = true
+upload_to_vcs_release = true
 upload_to_repository = false
 prerelease = true
 parser_angular_default_level_bump = "patch"
-parser_angular_patch_types = "fix,perf,docs,chore,chore(release)"
-build_command = "poetry build"
+patch_tags = "fix,perf,docs,chore,chore(release)"
+build_command = "pip install poetry && poetry build"
 commit_message = "chore(release): Tag v{version} [skip ci]"
```

### Comparing `secureli-0.8.0/secureli/abstractions/echo.py` & `secureli-0.8.1/secureli/abstractions/echo.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/abstractions/lexer_guesser.py` & `secureli-0.8.1/secureli/abstractions/lexer_guesser.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/abstractions/pre_commit.py` & `secureli-0.8.1/secureli/abstractions/pre_commit.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/action.py` & `secureli-0.8.1/secureli/actions/action.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/build.py` & `secureli-0.8.1/secureli/actions/build.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/initializer.py` & `secureli-0.8.1/secureli/actions/initializer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/scan.py` & `secureli-0.8.1/secureli/actions/scan.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/setup.py` & `secureli-0.8.1/secureli/actions/setup.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/actions/update.py` & `secureli-0.8.1/secureli/actions/update.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/container.py` & `secureli-0.8.1/secureli/container.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/main.py` & `secureli-0.8.1/secureli/main.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/repositories/repo_files.py` & `secureli-0.8.1/secureli/repositories/repo_files.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/repositories/secureli_config.py` & `secureli-0.8.1/secureli/repositories/secureli_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/repositories/settings.py` & `secureli-0.8.1/secureli/repositories/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/files/base-pre-commit.yaml` & `secureli-0.8.1/secureli/resources/files/base-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/files/build.txt` & `secureli-0.8.1/secureli/resources/files/build.txt`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/files/csharp-pre-commit.yaml` & `secureli-0.8.1/secureli/resources/files/csharp-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/files/javascript-pre-commit.yaml` & `secureli-0.8.1/secureli/resources/files/javascript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/files/typescript-pre-commit.yaml` & `secureli-0.8.1/secureli/resources/files/typescript-pre-commit.yaml`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/read_resource.py` & `secureli-0.8.1/secureli/resources/read_resource.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/resources/slugify.py` & `secureli-0.8.1/secureli/resources/slugify.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/git_ignore.py` & `secureli-0.8.1/secureli/services/git_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/language_analyzer.py` & `secureli-0.8.1/secureli/services/language_analyzer.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/language_config.py` & `secureli-0.8.1/secureli/services/language_config.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/language_support.py` & `secureli-0.8.1/secureli/services/language_support.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/logging.py` & `secureli-0.8.1/secureli/services/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,21 +93,23 @@
 
         return log_entry
 
     def failure(
         self,
         action: LogAction,
         details: str,
-        total_failure_count: Optional[int],
-        individual_failure_count: Optional[object],
+        total_failure_count: Optional[int] = None,
+        individual_failure_count: Optional[object] = None,
     ) -> LogEntry:
         """
         Capture a failure against an action, with details
         :param action: The action that failed
         :param details: Details about the failure
+        :param total_failure_count: The total failure count
+        :param individual_failure_count: The individual failure count
         """
         secureli_config = self.secureli_config.load()
         hook_config = (
             None
             if not secureli_config.languages
             else self.language_support.get_configuration(secureli_config.languages)
         )
```

### Comparing `secureli-0.8.0/secureli/services/scanner.py` & `secureli-0.8.1/secureli/services/scanner.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/secureli_ignore.py` & `secureli-0.8.1/secureli/services/secureli_ignore.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/services/updater.py` & `secureli-0.8.1/secureli/services/updater.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/settings.py` & `secureli-0.8.1/secureli/settings.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/utilities/git_meta.py` & `secureli-0.8.1/secureli/utilities/git_meta.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/utilities/patterns.py` & `secureli-0.8.1/secureli/utilities/patterns.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/secureli/utilities/usage_stats.py` & `secureli-0.8.1/secureli/utilities/usage_stats.py`

 * *Files identical despite different names*

### Comparing `secureli-0.8.0/PKG-INFO` & `secureli-0.8.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: secureli
-Version: 0.8.0
+Version: 0.8.1
 Summary: Secure Project Manager
 License: Apache-2.0
 Author: Caleb Tonn
 Author-email: caleb.tonn@slalom.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -36,45 +36,47 @@
 - installs linters based on the code of your project to support security and coding best practices
 - configures all the hooks needed so you don’t have to
 
 SeCureLI isn’t a magic tool that makes things secure because you have it. It enables a lot of other tools that you could set up individually and helps you as a builder write better code.
 
 Looking to contribute? Read our [CONTRIBUTING.md](https://github.com/slalombuild/secureli/blob/main/CONTRIBUTING.md)
 
-# Installation and Usage
+# Installation
 
-## Secureli Installation via Homebrew
+## Homebrew
 
-Current the only packaging tool that is supported for Secureli is Homebrew. To install secureli via homebrew, issue the following commands
+To install seCureLI via homebrew, issue the following commands
 
 ```commandline
 brew tap slalombuild/secureli
 brew install secureli
 ```
 
-## Upgrading Secureli via Homebrew
+## pip (Package Installer for Python)
 
-To update secureli, you can use the standard homebrew update command to pull down the latest formula
+To install seCureLI via pip, issue the following commands
 
 ```commandline
-brew update
+pip install secureli
 ```
 
 # Usage
 
-Once installed you can see the latest documentation for SeCureLI by entering the following on a command prompt:
+## Help
+
+Once installed you can see the latest documentation for seCureLI by entering the following on a command prompt:
 
 ```python
 % secureli --help
 ```
 
 You will see a list of commands and descriptions of each. You can also pull up documentation for each command with the same pattern. For example:
 
 ```python
-(secureli-py3.9) tristan@Tristans-MacBook-Pro secureli % secureli init --help
+% secureli init --help
 
  Usage: secureli init [OPTIONS]
 
  Detect languages and initialize pre-commit hooks and linters for the project
 
 ╭─ Options ──────────────────────────────────────────────────────────────────────────────────────╮
 │ --reset  -r        Disregard the installed configuration, if any, and treat as a new install   │
@@ -85,83 +87,120 @@
 
 When invoking these commands, you can combine the short versions into a single flag. For example, the following commands are equivalent:
 
 ```python
 % secureli init --reset --yes
 % secureli init -ry
 ```
+## Init
 
-# Tutorial to Use Observability Platform to Show Usage Statistics
+After seCureLI is installed, you can use it to configure your local git repository with a set of pre-commit hooks appropriate for your repo, based on the languages found in your repo's source code files.
 
-This tutorial uses New Relic as the sample observability platform. Other platforms may also work, but have not been tested.
-Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+All you need to do is run:
 
-## Steps
+```commandline
+% secureli init
+```
 
-- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
-- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
-- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
-- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
-- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+Running secureli init will allow secureli to detect the languages in your repo, install pre-commit, install all the appropriate pre-commit hooks for your local repo, and run a scan for secrets in your local repo.
+
+# Upgrade
+
+## Upgrading seCureLI via Homebrew
+
+If you installed seCureLI using Homebrew, you can use the standard homebrew update command to pull down the latest formula.
 
 ```commandline
-FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+brew update
+```
+## Upgrading via pip
+
+If you installed seCureLI using pip, you can use the following command to upgrade to the latest version of seCureLI.
+
+```commandline
+pip install --upgrade secureli
+```
+## Upgrading pre-commit hooks for repo
+
+In order to upgrade to the latest released version of each pre-commit hook configured for your repo, use the following command.
+
+```commandline
+secureli update --latest
 ```
 
 # Configuration
 
-SeCureLI is configurable via a .secureli.yaml file present in the consuming repository.
+SeCureLI is configurable via a .secureli.yaml file present in the root of your local repository.
+
+## .secureli.yaml
 
-## .secureli.yaml - top level
+### top level
 
 | Key                | Description                                                                                                                      |
 | ------------------ | -------------------------------------------------------------------------------------------------------------------------------- |
 | `repo_files`       | Affects how SeCureLI will interpret the repository, both for language analysis and as it executes various linters.               |
 | `echo`             | Adjusts how SeCureLI will print information to the user.                                                                         |
 | `language_support` | Affects SeCureLI's language analysis and support phase.                                                                          |
 | `pre_commit`       | Enables various overrides and options for SeCureLI's configuration and usage of pre-commit, the underlying code analysis system. |
 
-## .secureli.yaml - repo_files
+### repo_files
 
 | Key                       | Description                                                                                                                                                                                                                                                             |
 | ------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `max_file_size`           | A number in bytes. Files over this size will not be considered during language analysis, for speed purposes. Default: 100000                                                                                                                                            |
 | `ignored_file_extensions` | Which file extensions not to consider during language analysis.                                                                                                                                                                                                         |
 | `exclude_file_patterns`   | Which file patterns to ignore during language analysis and code analysis execution. Use a typical file pattern you might find in a .gitignore file, such as `*.py` or `tests/`. Certain patterns you will have to wrap in double-quotes for the entry to be valid YAML. |
 
-## .secureli.yaml - echo
+### echo
 
 | Key     | Description                                                                                                                                        |
 | ------- | -------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `level` | The log level to display to the user. Defaults to ERROR, which includes `error` and `print` messages, without including warnings or info messages. |
 
-## .secureli.yaml - pre_commit
+### pre_commit
 
 | Key                | Description                                                                                                                                                                                                                               |
 | ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `repos`            | A set of template-based Pre-Commit Repos to configure with overrides, identified by URL. These override repo-configurations stored in the template, and attempting to modify a repo not configured into the template will have no effect. |
 | `suppressed_repos` | A set of template-based Pre-Commit Repo URLs to completely remove from the final configuration. These remove repo configurations stored in the template, removing a repo not stored in the template will be ignored.                      |
 
-## .secureli.yaml - pre_commit.repos
+### pre_commit.repos
 
 | Key                   | Description                                                                                                                                            |
 | --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
 | `url`                 | The identifying URL of the repo being leveraged by pre-commit, within which one or more hooks can be leveraged.                                        |
 | `hooks`               | A set of hooks associated with the specified repository to override. See the next section for what we can configure there.                             |
 | `suppressed_hook_ids` | A set of hook IDs to remove from the repository as configured within the template. Hook IDs not present in the template configuration will be ignored. |
 
-## .secureli.yaml - pre_commit.repos.hooks
+### pre_commit.repos.hooks
 
 | Key                     | Description                                                                                                                                                                                                                                                                  |
 | ----------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
 | `id`                    | The identifying string of the pre-commit hook to override.                                                                                                                                                                                                                   |
 | `arguments`             | A set of arguments to provide to the pre-commit hook identified by `id`. These arguments overwrite any existing arguments.                                                                                                                                                   |
 | `additional_args`       | A set of arguments to provide to the pre-commit hook identified by `id`. These arguments are appended after an existing arguments.                                                                                                                                           |
 | `exclude_file_patterns` | A set of file patterns to provide to pre-commit to ignore for the purposes of this hook. Use a typical file pattern you might find in a .gitignore file, such as `*.py` or `tests/`. Certain patterns you will have to wrap in double-quotes for the entry to be valid YAML. |
 
+## Using Observability Platform to Show Secret Detection Statistics
+
+SeCureLI can send secret detection events to an observability platform, such as New Relic.  Other platforms may also work, but have not been tested.
+Should you need seCureLI to work with other platforms, please create a new issue in github, or contribute to the open source project.
+
+### Steps for New Relic
+
+- Assuming, seCureLI has been setup and installed, sign up to New Relic Log Platform https://docs.newrelic.com/docs/logs/log-api/introduction-log-api/
+- Retrieve API_KEY and API_ENDPOINT from New Relic. API_ENDPOINT for New Relic should be https://log-api.newrelic.com/log/v1
+- On your development machine, setup environment variable with variable name API_KEY and API_ENDPOINT
+- Once the above setup is complete, everytime seCureLI triggered, it should send a usage log to New Relic
+- In New Relic, you can create a dashboard of metric to see the number of times secret was caught using query such as
+
+```commandline
+FROM Log Select sum(failure_count_details.detect_secrets) as 'Caught Secret Count'
+```
+
 ## License
 
 Copyright 2023 Slalom, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

