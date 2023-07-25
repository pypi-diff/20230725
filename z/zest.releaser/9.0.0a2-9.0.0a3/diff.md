# Comparing `tmp/zest.releaser-9.0.0a2.tar.gz` & `tmp/zest.releaser-9.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zest.releaser-9.0.0a2.tar", last modified: Wed Jul 19 21:52:28 2023, max compression
+gzip compressed data, was "zest.releaser-9.0.0a3.tar", last modified: Tue Jul 25 15:44:42 2023, max compression
```

## Comparing `zest.releaser-9.0.0a2.tar` & `zest.releaser-9.0.0a3.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.468669 zest.releaser-9.0.0a2/
--rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      938 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/CREDITS.rst
--rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/LICENSE.rst
--rw-r--r--   0 maurits    (501) staff       (20)      149 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    14946 2023-07-19 21:52:28.468859 zest.releaser-9.0.0a2/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     8076 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.445818 zest.releaser-9.0.0a2/doc/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.453175 zest.releaser-9.0.0a2/doc/source/
--rw-r--r--   0 maurits    (501) staff       (20)     2010 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/assumptions.rst
--rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/changelog.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6894 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/conf.py
--rw-r--r--   0 maurits    (501) staff       (20)       32 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/credits.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/developing.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8122 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/entrypoints.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/further_reading.rst
--rw-r--r--   0 maurits    (501) staff       (20)      837 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/index.rst
--rw-r--r--   0 maurits    (501) staff       (20)     6941 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/options.rst
--rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/overview.rst
--rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/project.rst
--rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/uploading.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3566 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/doc/source/versions.rst
--rw-r--r--   0 maurits    (501) staff       (20)     3378 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)      294 2023-07-19 21:52:28.469385 zest.releaser-9.0.0a2/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)      251 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/tox.ini
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.446213 zest.releaser-9.0.0a2/zest/
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.460146 zest.releaser-9.0.0a2/zest/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/addchangelogentry.py
--rw-r--r--   0 maurits    (501) staff       (20)    17679 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/baserelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     6297 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/bumpversion.py
--rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/choose.py
--rw-r--r--   0 maurits    (501) staff       (20)      962 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/fullrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     4178 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/git.py
--rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/lasttagdiff.py
--rw-r--r--   0 maurits    (501) staff       (20)      833 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/lasttaglog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1939 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/longtest.py
--rw-r--r--   0 maurits    (501) staff       (20)     5172 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/postrelease.py
--rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/preparedocs.py
--rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/prerelease.py
--rw-r--r--   0 maurits    (501) staff       (20)    24188 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)    13543 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.468418 zest.releaser-9.0.0a2/zest/releaser/tests/
--rw-r--r--   0 maurits    (501) staff       (20)       10 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/addchangelogentry.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4446 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/baserelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/bumpversion.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/choose.txt
--rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/cmd_error.py
--rw-r--r--   0 maurits    (501) staff       (20)    17408 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/example.tar
--rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/fullrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/functional-git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4444 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/functional-with-hooks.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4311 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/functional.py
--rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/git.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/postrelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/preparedocs.txt
--rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/prerelease.txt
--rw-r--r--   0 maurits    (501) staff       (20)    12174 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypi.txt
--rw-r--r--   0 maurits    (501) staff       (20)      203 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_both.txt
--rw-r--r--   0 maurits    (501) staff       (20)      275 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_new.txt
--rw-r--r--   0 maurits    (501) staff       (20)      109 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_no_input.txt
--rw-r--r--   0 maurits    (501) staff       (20)      107 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_no_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)       57 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_old.txt
--rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_simple.txt
--rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_universal_nocreate.txt
--rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pypirc_yes_release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4211 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pyproject-toml.txt
--rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)     3118 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/release.txt
--rw-r--r--   0 maurits    (501) staff       (20)     2857 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/test_setup.py
--rw-r--r--   0 maurits    (501) staff       (20)    22286 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/utils.txt
--rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/tests/vcs.txt
--rw-r--r--   0 maurits    (501) staff       (20)    33247 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/utils.py
--rw-r--r--   0 maurits    (501) staff       (20)    18085 2023-07-19 21:52:27.000000 zest.releaser-9.0.0a2/zest/releaser/vcs.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-19 21:52:28.455045 zest.releaser-9.0.0a2/zest.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    14946 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     2238 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      951 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      220 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-19 21:52:28.000000 zest.releaser-9.0.0a2/zest.releaser.egg-info/top_level.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.452868 zest.releaser-9.0.0a3/
+-rw-r--r--   0 maurits    (501) staff       (20)     5088 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1288 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1071 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/CREDITS.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    17987 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      756 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/LICENSE.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      149 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    15569 2023-07-25 15:44:42.453047 zest.releaser-9.0.0a3/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     8076 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.429459 zest.releaser-9.0.0a3/doc/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.437101 zest.releaser-9.0.0a3/doc/source/
+-rw-r--r--   0 maurits    (501) staff       (20)     2010 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/assumptions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)    50612 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/changelog.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6894 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/conf.py
+-rw-r--r--   0 maurits    (501) staff       (20)       32 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/credits.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3191 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/developing.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8341 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/entrypoints.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1265 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/further_reading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      837 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/index.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     6941 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/options.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       30 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/overview.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     1165 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/project.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     9536 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/uploading.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3566 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/doc/source/versions.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     3378 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)      294 2023-07-25 15:44:42.453638 zest.releaser-9.0.0a3/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      146 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)      251 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.429855 zest.releaser-9.0.0a3/zest/
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.444042 zest.releaser-9.0.0a3/zest/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      398 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3063 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/addchangelogentry.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17830 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/baserelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     6297 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/bumpversion.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1241 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/choose.py
+-rw-r--r--   0 maurits    (501) staff       (20)      962 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/fullrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4178 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/git.py
+-rw-r--r--   0 maurits    (501) staff       (20)      831 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/lasttagdiff.py
+-rw-r--r--   0 maurits    (501) staff       (20)      833 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/lasttaglog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1939 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/longtest.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5172 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/postrelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2146 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/preparedocs.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4590 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/prerelease.py
+-rw-r--r--   0 maurits    (501) staff       (20)    24188 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)    13543 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.452609 zest.releaser-9.0.0a3/zest/releaser/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)       10 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3657 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/addchangelogentry.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4446 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/baserelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4598 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/bumpversion.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1199 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/choose.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      122 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/cmd_error.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17408 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/example.tar
+-rw-r--r--   0 maurits    (501) staff       (20)     3166 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/fullrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     3936 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional-git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4444 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional-with-hooks.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4311 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/functional.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5662 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/git.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9742 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/postrelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1891 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/preparedocs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     1172 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/prerelease.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    12174 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypi.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      203 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_both.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      275 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_new.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      109 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_no_input.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_no_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       57 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_old.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       37 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_simple.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      155 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_universal_nocreate.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      127 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pypirc_yes_release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4211 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pyproject-toml.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      400 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     3118 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/release.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     2857 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/test_setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)    22286 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/utils.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     9600 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/tests/vcs.txt
+-rw-r--r--   0 maurits    (501) staff       (20)    33481 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)    18085 2023-07-25 15:44:41.000000 zest.releaser-9.0.0a3/zest/releaser/vcs.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-07-25 15:44:42.439075 zest.releaser-9.0.0a3/zest.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    15569 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     2238 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      951 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      220 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        5 2023-07-25 15:44:42.000000 zest.releaser-9.0.0a3/zest.releaser.egg-info/top_level.txt
```

### Comparing `zest.releaser-9.0.0a2/CHANGES.rst` & `zest.releaser-9.0.0a3/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog for zest.releaser
 ===========================
 
+9.0.0a3 (2023-07-25)
+--------------------
+
+- Updated contributors list.
+
+- Documenting ``hook_package_dir`` setting for entry points (which isn't
+  needed for most entry points, btw).
+  Fixes `issue 370 <https://github.com/zestsoftware/zest.releaser/issues/370>`_.
+
+- Allowing for retry for ``git push``, which might fail because of a protected
+  branch. Also displaying that possible cause when it occurs. Fixes `issue 385
+  <https://github.com/zestsoftware/zest.releaser/issues/385>`_.
+
+
 9.0.0a2 (2023-07-19)
 --------------------
 
 - Ignore error output when calling `build`.
   We only need to look at the exit code to see if it worked.
   You can call zest.releaser with ``--verbose`` if you want
   to see the possible warnings.
```

### Comparing `zest.releaser-9.0.0a2/CONTRIBUTING.rst` & `zest.releaser-9.0.0a3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/CREDITS.rst` & `zest.releaser-9.0.0a3/CREDITS.rst`

 * *Files 19% similar despite different names*

```diff
@@ -18,7 +18,10 @@
   /tags for subversion.
 
 * `Richard Mitchell <https://github.com/mitchellrj>`_
   (`Isotoma <https://www.isotoma.com/>`_) added Python 3 support.
 
 * `Mateusz Legięcki <https://github.com/Behoston>`_ added a dockerfile for
   much easier testing.
+
+* `Eli Sallé <https://github.com/elisallenens>`_ added pyproject.toml support
+  for zest.releaser's own options. We're modern now!
```

### Comparing `zest.releaser-9.0.0a2/LICENSE.GPL` & `zest.releaser-9.0.0a3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/LICENSE.rst` & `zest.releaser-9.0.0a3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/PKG-INFO` & `zest.releaser-9.0.0a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 9.0.0a2
+Version: 9.0.0a3
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
@@ -239,17 +239,34 @@
 
 * `Richard Mitchell <https://github.com/mitchellrj>`_
   (`Isotoma <https://www.isotoma.com/>`_) added Python 3 support.
 
 * `Mateusz Legięcki <https://github.com/Behoston>`_ added a dockerfile for
   much easier testing.
 
+* `Eli Sallé <https://github.com/elisallenens>`_ added pyproject.toml support
+  for zest.releaser's own options. We're modern now!
+
 Changelog for zest.releaser
 ===========================
 
+9.0.0a3 (2023-07-25)
+--------------------
+
+- Updated contributors list.
+
+- Documenting ``hook_package_dir`` setting for entry points (which isn't
+  needed for most entry points, btw).
+  Fixes `issue 370 <https://github.com/zestsoftware/zest.releaser/issues/370>`_.
+
+- Allowing for retry for ``git push``, which might fail because of a protected
+  branch. Also displaying that possible cause when it occurs. Fixes `issue 385
+  <https://github.com/zestsoftware/zest.releaser/issues/385>`_.
+
+
 9.0.0a2 (2023-07-19)
 --------------------
 
 - Ignore error output when calling `build`.
   We only need to look at the exit code to see if it worked.
   You can call zest.releaser with ``--verbose`` if you want
   to see the possible warnings.
```

### Comparing `zest.releaser-9.0.0a2/README.rst` & `zest.releaser-9.0.0a3/README.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/assumptions.rst` & `zest.releaser-9.0.0a3/doc/source/assumptions.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/changelog.rst` & `zest.releaser-9.0.0a3/doc/source/changelog.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/conf.py` & `zest.releaser-9.0.0a3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/developing.rst` & `zest.releaser-9.0.0a3/doc/source/developing.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/entrypoints.rst` & `zest.releaser-9.0.0a3/doc/source/entrypoints.rst`

 * *Files 3% similar despite different names*

```diff
@@ -110,14 +110,17 @@
 
 * Entry-points given in ``setup.cfg`` will be processed before
   entry-point defined via installed packages.
 
 * The order in which entry-point defined via installed packages are
   processed is undefined.
 
+* *If* you use an entry point defined in the package you're releasing *and*
+  your package has the code inside a ``src/`` dir, you might have to add
+  ``hook_package_dir = src`` to the ``[tool.zest-releaser]`` section.
 
 
 Comments about data dict items
 ------------------------------
 
 Your entry point gets a data dictionary: the items you get in that dictionary
 are documented below.  Some comments about them:
```

### Comparing `zest.releaser-9.0.0a2/doc/source/further_reading.rst` & `zest.releaser-9.0.0a3/doc/source/further_reading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/index.rst` & `zest.releaser-9.0.0a3/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/options.rst` & `zest.releaser-9.0.0a3/doc/source/options.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/project.rst` & `zest.releaser-9.0.0a3/doc/source/project.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/uploading.rst` & `zest.releaser-9.0.0a3/doc/source/uploading.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/doc/source/versions.rst` & `zest.releaser-9.0.0a3/doc/source/versions.rst`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/pyproject.toml` & `zest.releaser-9.0.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 # See https://snarky.ca/what-the-heck-is-pyproject-toml/
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "zest.releaser"
-version = "9.0.0a2"
+version = "9.0.0a3"
 description = "Software releasing made easy and repeatable"
 license = {text = "GPL"}
 authors = [
     {name = "Reinout van Rees", email = "reinout@vanrees.org"},
     {name = "Maurits van Rees", email = "maurits@vanrees.org"},
 ]
 dependencies = [
```

### Comparing `zest.releaser-9.0.0a2/zest/releaser/addchangelogentry.py` & `zest.releaser-9.0.0a3/zest/releaser/addchangelogentry.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/baserelease.py` & `zest.releaser-9.0.0a3/zest/releaser/baserelease.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,15 +404,19 @@
         """Offer to push changes, if needed."""
         push_cmds = self.vcs.push_commands()
         if not push_cmds:
             return
         default_anwer = self.zest_releaser_config.push_changes()
         if utils.ask("OK to push commits to the server?", default=default_anwer):
             for push_cmd in push_cmds:
-                output = execute_command(push_cmd)
+                output = execute_command(
+                    push_cmd,
+                    allow_retry=True,
+                    fail_message="Perhaps the main branch is protected?",
+                )
                 logger.info(output)
 
     def _run_hooks(self, when):
         which_releaser = self.__class__.__name__.lower()
         utils.run_hooks(self.zest_releaser_config, which_releaser, when, self.data)
 
     def run(self):
```

### Comparing `zest.releaser-9.0.0a2/zest/releaser/bumpversion.py` & `zest.releaser-9.0.0a3/zest/releaser/bumpversion.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/choose.py` & `zest.releaser-9.0.0a3/zest/releaser/choose.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/fullrelease.py` & `zest.releaser-9.0.0a3/zest/releaser/fullrelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/git.py` & `zest.releaser-9.0.0a3/zest/releaser/git.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/lasttagdiff.py` & `zest.releaser-9.0.0a3/zest/releaser/lasttagdiff.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/lasttaglog.py` & `zest.releaser-9.0.0a3/zest/releaser/lasttaglog.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/longtest.py` & `zest.releaser-9.0.0a3/zest/releaser/longtest.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/postrelease.py` & `zest.releaser-9.0.0a3/zest/releaser/postrelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/preparedocs.py` & `zest.releaser-9.0.0a3/zest/releaser/preparedocs.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/prerelease.py` & `zest.releaser-9.0.0a3/zest/releaser/prerelease.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/pypi.py` & `zest.releaser-9.0.0a3/zest/releaser/pypi.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/release.py` & `zest.releaser-9.0.0a3/zest/releaser/release.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/addchangelogentry.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/addchangelogentry.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/baserelease.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/baserelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/bumpversion.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/bumpversion.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/choose.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/choose.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/example.tar` & `zest.releaser-9.0.0a3/zest/releaser/tests/example.tar`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/fullrelease.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/fullrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/functional-git.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/functional-git.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/functional-with-hooks.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/functional-with-hooks.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/functional.py` & `zest.releaser-9.0.0a3/zest/releaser/tests/functional.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/git.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/git.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/postrelease.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/postrelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/preparedocs.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/preparedocs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/prerelease.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/prerelease.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/pypi.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/pypi.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/pyproject-toml.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/pyproject-toml.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/release.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/release.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/test_setup.py` & `zest.releaser-9.0.0a3/zest/releaser/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/utils.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/utils.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/tests/vcs.txt` & `zest.releaser-9.0.0a3/zest/releaser/tests/vcs.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest/releaser/utils.py` & `zest.releaser-9.0.0a3/zest/releaser/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -736,14 +736,17 @@
     There is an error when there is a red color in the output.
 
     It might be a warning, but we cannot detect the distinction.
     """
     result = _execute_command(command, cwd=cwd, extra_environ=extra_environ)
     if not allow_retry:
         return result
+    if AUTO_RESPONSE:
+        # Also don't ask for retry, just return the result.
+        return result
     if Fore.RED not in result:
         show_interesting_lines(result)
         return result
     # There are warnings or errors. Print the complete result.
     print(result)
     print(Fore.RED + "There were errors or warnings.")
     if fail_message:
@@ -766,23 +769,28 @@
         result.append(
             execute_command(cmd, allow_retry=allow_retry, fail_message=fail_message)
         )
     return "\n".join(result)
 
 
 def retry_yes_no(command):
-    """Ask the user to maybe retry a command."""
+    """Ask the user to maybe retry a command.
+
+    This is used for the twine upload command and for the final 'git push'.
+
+    """
     explanation = """
     You have these options for retrying (first character is enough):
     Yes:   Retry. Do this if it looks like a temporary Internet or PyPI outage.
            You can also first edit $HOME/.pypirc and then retry in
            case of a credentials problem.
     No:    Do not retry, but continue with the rest of the process.
     Quit:  Stop completely. Note that the postrelease step has not
-           been run yet, you need to do that manually.
+           finished fully. You need to do the 'git push' and possibly the upload
+           manually.
     ?:     Show this help."""
     explanation = textwrap.dedent(explanation)
     question = "Retry this command? [Yes/no/quit/?]"
     if AUTO_RESPONSE:
         msg = (
             "The question '%s' requires a manual answer, but "
             "we're running in --no-input mode."
```

### Comparing `zest.releaser-9.0.0a2/zest/releaser/vcs.py` & `zest.releaser-9.0.0a3/zest/releaser/vcs.py`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest.releaser.egg-info/PKG-INFO` & `zest.releaser-9.0.0a3/zest.releaser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zest.releaser
-Version: 9.0.0a2
+Version: 9.0.0a3
 Summary: Software releasing made easy and repeatable
 Author-email: Reinout van Rees <reinout@vanrees.org>, Maurits van Rees <maurits@vanrees.org>
 License: GPL
 Project-URL: documentation, https://zestreleaser.readthedocs.io
 Project-URL: repository, https://github.com/zestsoftware/zest.releaser/
 Project-URL: changelog, https://github.com/zestsoftware/zest.releaser/blob/master/CHANGES.rst
 Keywords: releasing,packaging,pypi
@@ -239,17 +239,34 @@
 
 * `Richard Mitchell <https://github.com/mitchellrj>`_
   (`Isotoma <https://www.isotoma.com/>`_) added Python 3 support.
 
 * `Mateusz Legięcki <https://github.com/Behoston>`_ added a dockerfile for
   much easier testing.
 
+* `Eli Sallé <https://github.com/elisallenens>`_ added pyproject.toml support
+  for zest.releaser's own options. We're modern now!
+
 Changelog for zest.releaser
 ===========================
 
+9.0.0a3 (2023-07-25)
+--------------------
+
+- Updated contributors list.
+
+- Documenting ``hook_package_dir`` setting for entry points (which isn't
+  needed for most entry points, btw).
+  Fixes `issue 370 <https://github.com/zestsoftware/zest.releaser/issues/370>`_.
+
+- Allowing for retry for ``git push``, which might fail because of a protected
+  branch. Also displaying that possible cause when it occurs. Fixes `issue 385
+  <https://github.com/zestsoftware/zest.releaser/issues/385>`_.
+
+
 9.0.0a2 (2023-07-19)
 --------------------
 
 - Ignore error output when calling `build`.
   We only need to look at the exit code to see if it worked.
   You can call zest.releaser with ``--verbose`` if you want
   to see the possible warnings.
```

### Comparing `zest.releaser-9.0.0a2/zest.releaser.egg-info/SOURCES.txt` & `zest.releaser-9.0.0a3/zest.releaser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zest.releaser-9.0.0a2/zest.releaser.egg-info/entry_points.txt` & `zest.releaser-9.0.0a3/zest.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

