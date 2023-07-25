# Comparing `tmp/scmrepo-1.0.4.tar.gz` & `tmp/scmrepo-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scmrepo-1.0.4.tar", last modified: Tue Jun 20 06:26:29 2023, max compression
+gzip compressed data, was "scmrepo-1.1.0.tar", last modified: Tue Jul 25 08:13:13 2023, max compression
```

## Comparing `scmrepo-1.0.4.tar` & `scmrepo-1.1.0.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-20 06:26:07.000000 scmrepo-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-20 06:26:07.000000 scmrepo-1.0.4/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-20 06:26:07.000000 scmrepo-1.0.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-06-20 06:26:07.000000 scmrepo-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 06:26:29.901444 scmrepo-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-20 06:26:07.000000 scmrepo-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-20 06:26:07.000000 scmrepo-1.0.4/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 06:26:07.000000 scmrepo-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-20 06:26:29.901444 scmrepo-1.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.893444 scmrepo-1.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/asyn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/fs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/
--rw-r--r--   0 runner    (1001) docker     (123)    16230 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11413 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/
--rw-r--r--   0 runner    (1001) docker     (123)    29311 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8172 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    21888 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/gitpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/
--rw-r--r--   0 runner    (1001) docker     (123)    27611 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/git/stash.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-20 06:26:07.000000 scmrepo-1.0.4/src/scmrepo/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.897444 scmrepo-1.0.4/src/scmrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-20 06:26:29.000000 scmrepo-1.0.4/src/scmrepo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 06:26:29.901444 scmrepo-1.0.4/tests/git-init/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/git-init/git.sh
--rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_dulwich.py
--rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_fs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34105 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_git.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_noscm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_pygit2.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_scmrepo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/test_stash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/user.key
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-20 06:26:07.000000 scmrepo-1.0.4/tests/user.key.pub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.383854 scmrepo-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.383854 scmrepo-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-25 08:12:45.000000 scmrepo-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-25 08:12:45.000000 scmrepo-1.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-25 08:12:45.000000 scmrepo-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11340 2023-07-25 08:12:45.000000 scmrepo-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-25 08:13:13.387854 scmrepo-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-07-25 08:12:45.000000 scmrepo-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-25 08:12:45.000000 scmrepo-1.1.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 08:12:45.000000 scmrepo-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-25 08:13:13.391854 scmrepo-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.379854 scmrepo-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.383854 scmrepo-1.1.0/src/scmrepo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/fs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/src/scmrepo/git/
+-rw-r--r--   0 runner    (1001) docker     (123)    16393 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/src/scmrepo/git/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/
+-rw-r--r--   0 runner    (1001) docker     (123)    30257 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/asyncssh_vendor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22004 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/gitpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/src/scmrepo/git/backend/pygit2/
+-rw-r--r--   0 runner    (1001) docker     (123)    28672 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/pygit2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/backend/pygit2/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20986 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3569 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/git/stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-07-25 08:12:45.000000 scmrepo-1.1.0/src/scmrepo/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.383854 scmrepo-1.1.0/src/scmrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-25 08:13:13.000000 scmrepo-1.1.0/src/scmrepo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 08:13:13.387854 scmrepo-1.1.0/tests/git-init/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/git-init/git.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6745 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_dulwich.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5166 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_fs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34467 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_noscm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_pygit2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_scmrepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/test_stash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/user.key
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-25 08:12:45.000000 scmrepo-1.1.0/tests/user.key.pub
```

### Comparing `scmrepo-1.0.4/.cruft.json` & `scmrepo-1.1.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/.github/dependabot.yml` & `scmrepo-1.1.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/.github/workflows/release.yaml` & `scmrepo-1.1.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/.github/workflows/tests.yaml` & `scmrepo-1.1.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/.gitignore` & `scmrepo-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/.pre-commit-config.yaml` & `scmrepo-1.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/CODE_OF_CONDUCT.rst` & `scmrepo-1.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/CONTRIBUTING.rst` & `scmrepo-1.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/LICENSE` & `scmrepo-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/PKG-INFO` & `scmrepo-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.4
+Version: 1.1.0
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.4/README.rst` & `scmrepo-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/noxfile.py` & `scmrepo-1.1.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/pyproject.toml` & `scmrepo-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/setup.cfg` & `scmrepo-1.1.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 	pytest-sugar==0.9.5
 	pytest-cov==3.0.0
 	pytest-mock==3.8.2
 	pylint==2.15.0
 	mypy==0.971
 	pytest-test-utils==0.0.8
 	pytest-asyncio==0.18.3
-	pytest-docker==0.12.0; python_version < '3.10' or sys_platform != 'win32'
+	pytest-docker==0.12.0; python_version < '3.10' and implementation_name != 'pypy'
 	mock==5.0.1
 	paramiko==3.1.0
 	types-certifi==2021.10.8.3
 	types-mock==5.0.0.6
 	types-paramiko==3.0.0.10
 dev = 
 	%(tests)s
```

### Comparing `scmrepo-1.0.4/src/scmrepo/asyn.py` & `scmrepo-1.1.0/src/scmrepo/asyn.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/base.py` & `scmrepo-1.1.0/src/scmrepo/base.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/exceptions.py` & `scmrepo-1.1.0/src/scmrepo/exceptions.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/fs.py` & `scmrepo-1.1.0/src/scmrepo/fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/git/__init__.py` & `scmrepo-1.1.0/src/scmrepo/git/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,19 +131,22 @@
 
     @classmethod
     def clone(
         cls,
         url: str,
         to_path: str,
         rev: Optional[str] = None,
+        bare: bool = False,
+        mirror: bool = False,
         **kwargs,
     ):
+        assert not (rev and bare), "rev checkout is unsupported in bare repos"
         for _, backend in GitBackends.DEFAULT.items():
             try:
-                backend.clone(url, to_path, **kwargs)
+                backend.clone(url, to_path, bare=bare, mirror=mirror, **kwargs)
                 repo = cls(to_path)
                 if rev:
                     repo.checkout(rev)
                 return repo
             except _SKIPPABLE:
                 pass
         raise NoGitBackendError("clone")
```

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/base.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     @staticmethod
     @abstractmethod
     def clone(
         url: str,
         to_path: str,
         shallow_branch: Optional[str] = None,
         progress: Callable[["GitProgressEvent"], None] = None,
+        bare: bool = False,
+        mirror: bool = False,
     ):
         pass
 
     @staticmethod
     @abstractmethod
     def init(path: str, bare: bool = False) -> None:
         pass
```

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/__init__.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,35 +95,36 @@
 
     def write(self, msg: Union[str, bytes]) -> int:
         self(msg)
         return len(msg)
 
 
 def _get_ssh_vendor() -> "SSHVendor":
+    import shutil
     import sys
 
     from dulwich.client import SubprocessSSHVendor
 
     from .asyncssh_vendor import AsyncSSHVendor, get_unsupported_opts
 
     ssh_command = os.environ.get("GIT_SSH_COMMAND", os.environ.get("GIT_SSH"))
     if ssh_command:
         logger.debug("dulwich: Using environment GIT_SSH_COMMAND '%s'", ssh_command)
         return SubprocessSSHVendor()
 
-    if sys.platform == "win32" and os.environ.get("MSYSTEM"):
+    if sys.platform == "win32" and os.environ.get("MSYSTEM") and shutil.which("ssh"):
         # see https://github.com/iterative/dvc/issues/7702
         logger.debug(
             "dulwich: native win32 Python inside MSYS2/git-bash, using MSYS2 OpenSSH"
         )
         return SubprocessSSHVendor()
 
     default_config = os.path.expanduser(os.path.join("~", ".ssh", "config"))
     unsupported = list(get_unsupported_opts([default_config]))
-    if unsupported:
+    if unsupported and shutil.which("ssh"):
         logger.debug(
             "dulwich: unsupported SSH config option(s) '%s', using system OpenSSH",
             ", ".join(unsupported),
         )
         return SubprocessSSHVendor()
     return AsyncSSHVendor()
 
@@ -187,44 +188,52 @@
     @classmethod
     def clone(
         cls,
         url: str,
         to_path: str,
         shallow_branch: Optional[str] = None,
         progress: Callable[["GitProgressEvent"], None] = None,
+        bare: bool = False,
+        mirror: bool = False,
     ):
         from urllib.parse import urlparse
 
         from dulwich.porcelain import NoneStream
         from dulwich.porcelain import clone as git_clone
 
+        if mirror:
+            bare = True
         parsed = urlparse(url)
         try:
             clone_from = partial(
                 git_clone,
                 url,
                 target=to_path,
                 errstream=(
                     DulwichProgressReporter(progress) if progress else NoneStream()
                 ),
+                bare=bare,
             )
             if shallow_branch:
                 # NOTE: dulwich only supports shallow/depth for non-local
                 # clones. This differs from CLI git, where depth is used for
                 # file:// URLs but not direct local paths
                 if parsed.scheme in ("git", "git+ssh", "ssh", "http", "https"):
                     depth = 1
                 else:
                     depth = 0
                 repo = clone_from(depth=depth, branch=os.fsencode(shallow_branch))
             else:
                 repo = clone_from()
 
             with closing(repo):
-                cls._set_default_tracking_branch(repo)
+                if mirror:
+                    cls._set_mirror(repo, progress=progress)
+                else:
+                    cls._set_default_tracking_branch(repo)
         except Exception as exc:
             raise CloneError(url, to_path) from exc
 
     @staticmethod
     def _set_default_tracking_branch(repo: "Repo"):
         from dulwich.refs import LOCAL_BRANCH_PREFIX, parse_symref_value
 
@@ -236,14 +245,35 @@
             branch = ref[len(LOCAL_BRANCH_PREFIX) :]
             config = repo.get_config()
             section = ("branch", os.fsencode(branch))
             config.set(section, b"remote", b"origin")
             config.set(section, b"merge", ref)
 
     @staticmethod
+    def _set_mirror(
+        repo: "Repo", progress: Callable[["GitProgressEvent"], None] = None
+    ):
+        from dulwich.porcelain import NoneStream, fetch
+
+        config = repo.get_config()
+        section = config[(b"remote", b"origin")]
+        try:
+            del section[b"fetch"]
+        except KeyError:
+            pass
+        section[b"fetch"] = b"+refs/*:refs/*"
+        section[b"mirror"] = b"true"
+        config.write_to_path()
+        fetch(
+            repo,
+            remote_location=b"origin",
+            errstream=(DulwichProgressReporter(progress) if progress else NoneStream()),
+        )
+
+    @staticmethod
     def init(path: str, bare: bool = False) -> None:
         from dulwich.porcelain import init
 
         init(path, bare=bare)
 
     @property
     def dir(self) -> str:
```

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/dulwich/client.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/dulwich/client.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/gitpython.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/gitpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -142,14 +142,16 @@
 
     @staticmethod
     def clone(
         url: str,
         to_path: str,
         shallow_branch: Optional[str] = None,
         progress: Callable[["GitProgressEvent"], None] = None,
+        bare: bool = False,
+        mirror: bool = False,
     ):
         from git import Repo
         from git.exc import GitCommandError
 
         ld_key = "LD_LIBRARY_PATH"
 
         env = fix_env()
@@ -174,14 +176,16 @@
             clone_from = partial(
                 Repo.clone_from,
                 url,
                 to_path,
                 env=env,  # needed before we can fix it in __init__
                 no_single_branch=True,
                 progress=GitProgressReporter.wrap_fn(progress) if progress else None,
+                bare=bare,
+                mirror=mirror,
             )
             if shallow_branch is None:
                 tmp_repo = clone_from()
             else:
                 tmp_repo = clone_from(branch=shallow_branch, depth=1)
             tmp_repo.close()
         except GitCommandError as exc:  # pylint: disable=no-member
```

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/__init__.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/pygit2/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from scmrepo.utils import relpath
 
 logger = logging.getLogger(__name__)
 
 
 if TYPE_CHECKING:
     from pygit2.remote import Remote  # type: ignore
+    from pygit2.repository import Repository
 
     from scmrepo.progress import GitProgressEvent
 
 
 class Pygit2Object(GitObject):
     def __init__(self, obj):
         self.obj = obj
@@ -150,34 +151,60 @@
     def release_odb_handles(self):
         yield
         # It is safe to free the libgit2 repo context multiple times - free
         # just forces libgit/pygit to release git ODB related contexts which
         # can be reacquired later as needed.
         self.repo.free()
 
-    @staticmethod
+    @classmethod
     def clone(
+        cls,
         url: str,
         to_path: str,
         shallow_branch: Optional[str] = None,
         progress: Callable[["GitProgressEvent"], None] = None,
+        bare: bool = False,
+        mirror: bool = False,
     ):
         from pygit2 import GitError, clone_repository
 
         from .callbacks import RemoteCallbacks
 
         if shallow_branch:
             raise NotImplementedError
+        if mirror:
+            bare = True
         try:
             with RemoteCallbacks(progress=progress) as cb:
-                clone_repository(url, to_path, callbacks=cb)
+                repo = clone_repository(url, to_path, callbacks=cb, bare=bare)
+                if mirror:
+                    cls._set_mirror(repo, progress=progress)
         except GitError as exc:
             raise CloneError(url, to_path) from exc
 
     @staticmethod
+    def _set_mirror(
+        repo: "Repository",
+        progress: Callable[["GitProgressEvent"], None] = None,
+    ):
+        from .callbacks import RemoteCallbacks
+
+        url = repo.remotes["origin"].url
+        repo.remotes.delete("origin")
+        # NOTE: Pygit2 remotes.create("origin", url, fetch_refspec) creates a
+        # duplicate config section for each remote config entry. We just edit
+        # the config directly so that it creates a single section to be
+        # consistent with CLI Git
+        repo.config["remote.origin.url"] = url
+        repo.config["remote.origin.fetch"] = "+refs/*:refs/*"
+        repo.config["remote.origin.mirror"] = True
+        with RemoteCallbacks(progress=progress) as cb:
+            repo.remotes["origin"].fetch(callbacks=cb)
+
+    @staticmethod
     def init(path: str, bare: bool = False) -> None:
         from pygit2 import init_repository
 
         init_repository(path, bare=bare)
 
     @property
     def dir(self) -> str:
```

### Comparing `scmrepo-1.0.4/src/scmrepo/git/backend/pygit2/callbacks.py` & `scmrepo-1.1.0/src/scmrepo/git/backend/pygit2/callbacks.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/git/credentials.py` & `scmrepo-1.1.0/src/scmrepo/git/credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/git/objects.py` & `scmrepo-1.1.0/src/scmrepo/git/objects.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/git/stash.py` & `scmrepo-1.1.0/src/scmrepo/git/stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/progress.py` & `scmrepo-1.1.0/src/scmrepo/progress.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo/utils.py` & `scmrepo-1.1.0/src/scmrepo/utils.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo.egg-info/PKG-INFO` & `scmrepo-1.1.0/src/scmrepo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scmrepo
-Version: 1.0.4
+Version: 1.1.0
 Summary: SCM wrapper and fsspec filesystem for Git for use in DVC
 Home-page: https://github.com/iterative/scmrepo
 Maintainer-email: support@dvc.org
 License: Apache-2.0
 Platform: any
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `scmrepo-1.0.4/src/scmrepo.egg-info/SOURCES.txt` & `scmrepo-1.1.0/src/scmrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/src/scmrepo.egg-info/requires.txt` & `scmrepo-1.1.0/src/scmrepo.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
 types-paramiko==3.0.0.10
 
-[dev:python_version < "3.10" or sys_platform != "win32"]
+[dev:python_version < "3.10" and implementation_name != "pypy"]
 pytest-docker==0.12.0
 
 [tests]
 pytest==7.2.0
 pytest-sugar==0.9.5
 pytest-cov==3.0.0
 pytest-mock==3.8.2
@@ -37,9 +37,9 @@
 pytest-asyncio==0.18.3
 mock==5.0.1
 paramiko==3.1.0
 types-certifi==2021.10.8.3
 types-mock==5.0.0.6
 types-paramiko==3.0.0.10
 
-[tests:python_version < "3.10" or sys_platform != "win32"]
+[tests:python_version < "3.10" and implementation_name != "pypy"]
 pytest-docker==0.12.0
```

### Comparing `scmrepo-1.0.4/tests/conftest.py` & `scmrepo-1.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_credentials.py` & `scmrepo-1.1.0/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_dulwich.py` & `scmrepo-1.1.0/tests/test_dulwich.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_fs.py` & `scmrepo-1.1.0/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_git.py` & `scmrepo-1.1.0/tests/test_git.py`

 * *Files 1% similar despite different names*

```diff
@@ -903,31 +903,45 @@
     assert git.get_ref("refs/heads/master") == rev
     scm.checkout("master")
     assert (tmp_dir / "foo").read_text() == "foo"
 
 
 @pytest.mark.parametrize("scheme", ["", "file://"])
 @pytest.mark.parametrize("shallow_branch", [None, "master"])
+@pytest.mark.parametrize("bare", [True, False])
 def test_clone(
     tmp_dir: TmpDir,
     scm: Git,
     git: Git,
     tmp_dir_factory: TempDirFactory,
     scheme: str,
     shallow_branch: Optional[str],
+    bare: bool,
 ):
     tmp_dir.gen("foo", "foo")
     scm.add_commit("foo", message="init")
     rev = scm.get_rev()
 
     target_dir = tmp_dir_factory.mktemp("git-clone")
-    git.clone(f"{scheme}{tmp_dir}", str(target_dir), shallow_branch=shallow_branch)
+    git.clone(
+        f"{scheme}{tmp_dir}",
+        str(target_dir),
+        shallow_branch=shallow_branch,
+        bare=bare,
+    )
     target = Git(str(target_dir))
     assert target.get_rev() == rev
-    assert (target_dir / "foo").read_text() == "foo"
+    if bare:
+        assert not (target_dir / "foo").exists()
+    else:
+        assert (target_dir / "foo").read_text() == "foo"
+        assert (target_dir / "foo").read_text() == "foo"
+    fs = target.get_fs(rev)
+    with fs.open("foo", mode="r") as fobj:
+        assert fobj.read().strip() == "foo"
 
 
 @pytest.mark.skip_git_backend("pygit2")
 def test_fetch(tmp_dir: TmpDir, scm: Git, git: Git, tmp_dir_factory: TempDirFactory):
     tmp_dir.gen("foo", "foo")
     scm.add_commit("foo", message="init")
```

### Comparing `scmrepo-1.0.4/tests/test_noscm.py` & `scmrepo-1.1.0/tests/test_noscm.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_pygit2.py` & `scmrepo-1.1.0/tests/test_pygit2.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_scmrepo.py` & `scmrepo-1.1.0/tests/test_scmrepo.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/test_stash.py` & `scmrepo-1.1.0/tests/test_stash.py`

 * *Files identical despite different names*

### Comparing `scmrepo-1.0.4/tests/user.key` & `scmrepo-1.1.0/tests/user.key`

 * *Files identical despite different names*

