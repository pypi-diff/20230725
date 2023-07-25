# Comparing `tmp/nabs-1.5.3.tar.gz` & `tmp/nabs-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nabs-1.5.3.tar", last modified: Tue Apr  4 21:41:42 2023, max compression
+gzip compressed data, was "nabs-1.5.4.tar", last modified: Tue Jul 25 21:21:41 2023, max compression
```

## Comparing `nabs-1.5.3.tar` & `nabs-1.5.4.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.302133 nabs-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (122)      128 2023-04-04 21:41:26.000000 nabs-1.5.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (122)      972 2023-04-04 21:41:26.000000 nabs-1.5.3/.flake8
--rw-r--r--   0 runner    (1001) docker     (122)      125 2023-04-04 21:41:26.000000 nabs-1.5.3/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (122)       32 2023-04-04 21:41:26.000000 nabs-1.5.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/.github/
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (122)     1205 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      746 2023-04-04 21:41:26.000000 nabs-1.5.3/.github/workflows/standard.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-04-04 21:41:26.000000 nabs-1.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-04-04 21:41:26.000000 nabs-1.5.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-04-04 21:41:26.000000 nabs-1.5.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-04-04 21:41:26.000000 nabs-1.5.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-04-04 21:41:26.000000 nabs-1.5.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (122)      193 2023-04-04 21:41:26.000000 nabs-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-04-04 21:41:42.298133 nabs-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-04-04 21:41:26.000000 nabs-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/conda-recipe/
--rw-r--r--   0 runner    (1001) docker     (122)      797 2023-04-04 21:41:26.000000 nabs-1.5.3/conda-recipe/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-04 21:41:26.000000 nabs-1.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (122)      606 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (122)      571 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/pre-release-notes.sh
--rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/release_notes.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (122)       55 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.290133 nabs-1.5.3/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (122)      106 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      697 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/optimize.rst
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/plans.rst
--rw-r--r--   0 runner    (1001) docker     (122)     7156 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/releases.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_changes.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.294133 nabs-1.5.3/docs/source/upcoming_release_notes/
--rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_release_notes/template-full.rst
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/source/upcoming_release_notes/template-short.rst
--rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-04-04 21:41:26.000000 nabs-1.5.3/docs/view-build.sh
--rw-r--r--   0 runner    (1001) docker     (122)       45 2023-04-04 21:41:26.000000 nabs-1.5.3/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs/
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      160 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     6597 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     9809 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/optimize.py
--rw-r--r--   0 runner    (1001) docker     (122)     6014 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/plan_stubs.py
--rw-r--r--   0 runner    (1001) docker     (122)    37406 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/plans.py
--rw-r--r--   0 runner    (1001) docker     (122)    13326 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     7874 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/simulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_callbacks.py
--rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_plan_stubs.py
--rw-r--r--   0 runner    (1001) docker     (122)    16821 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_plans.py
--rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_preprocessors.py
--rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_simulators.py
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/tests/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (122)     4836 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-04-04 21:41:26.000000 nabs-1.5.3/nabs/visualizations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-04 21:41:42.298133 nabs-1.5.3/nabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3712 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-04-04 21:41:42.000000 nabs-1.5.3/nabs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1110 2023-04-04 21:41:26.000000 nabs-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-04-04 21:41:26.000000 nabs-1.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-04 21:41:42.302133 nabs-1.5.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.145725 nabs-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (122)      128 2023-07-25 21:21:19.000000 nabs-1.5.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-07-25 21:21:19.000000 nabs-1.5.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-07-25 21:21:19.000000 nabs-1.5.4/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-07-25 21:21:19.000000 nabs-1.5.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1068 2023-07-25 21:21:19.000000 nabs-1.5.4/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-07-25 21:21:19.000000 nabs-1.5.4/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      767 2023-07-25 21:21:19.000000 nabs-1.5.4/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1241 2023-07-25 21:21:19.000000 nabs-1.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-07-25 21:21:19.000000 nabs-1.5.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-25 21:21:19.000000 nabs-1.5.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2969 2023-07-25 21:21:19.000000 nabs-1.5.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-07-25 21:21:19.000000 nabs-1.5.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      193 2023-07-25 21:21:19.000000 nabs-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-07-25 21:21:41.145725 nabs-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-07-25 21:21:19.000000 nabs-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)      798 2023-07-25 21:21:19.000000 nabs-1.5.4/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-25 21:21:19.000000 nabs-1.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      606 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      571 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2848 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.137725 nabs-1.5.4/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.133725 nabs-1.5.4/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.141725 nabs-1.5.4/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5842 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      697 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2487 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/optimize.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/plans.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     7299 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.141725 nabs-1.5.4/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1030 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/source/upcoming_release_notes/template-short.rst
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-07-25 21:21:19.000000 nabs-1.5.4/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-07-25 21:21:19.000000 nabs-1.5.4/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.141725 nabs-1.5.4/nabs/
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-07-25 21:21:40.000000 nabs-1.5.4/nabs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6597 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9809 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6014 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37406 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13326 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7874 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/simulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3212 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.145725 nabs-1.5.4/nabs/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3457 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2374 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3007 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3628 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_plan_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16821 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_plans.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4613 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_preprocessors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2394 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_simulators.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/tests/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4836 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2386 2023-07-25 21:21:19.000000 nabs-1.5.4/nabs/visualizations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-25 21:21:41.141725 nabs-1.5.4/nabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3715 2023-07-25 21:21:41.000000 nabs-1.5.4/nabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1412 2023-07-25 21:21:41.000000 nabs-1.5.4/nabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-25 21:21:41.000000 nabs-1.5.4/nabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-07-25 21:21:41.000000 nabs-1.5.4/nabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-25 21:21:41.000000 nabs-1.5.4/nabs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-07-25 21:21:19.000000 nabs-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-07-25 21:21:19.000000 nabs-1.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-25 21:21:41.145725 nabs-1.5.4/setup.cfg
```

### Comparing `nabs-1.5.3/.flake8` & `nabs-1.5.4/.flake8`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/.github/ISSUE_TEMPLATE.md` & `nabs-1.5.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/.github/PULL_REQUEST_TEMPLATE.md` & `nabs-1.5.4/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 9% similar despite different names*

```diff
@@ -20,10 +20,10 @@
 -->
 
 ## Pre-merge checklist
 - [ ] Code works interactively
 - [ ] Code contains descriptive docstrings, including context and API
 - [ ] New/changed functions and methods are covered in the test suite where possible
 - [ ] Test suite passes locally
-- [ ] Test suite passes on travis
+- [ ] Test suite passes on GitHub Actions
 - [ ] Ran docs/pre-release-notes.sh and created a pre-release documentation page
 - [ ] Pre-release docs include context, functional descriptions, and contributors as appropriate
```

### Comparing `nabs-1.5.3/.github/workflows/standard.yml` & `nabs-1.5.4/.github/workflows/standard.yml`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
   release:
     types:
       - created
 
 jobs:
   standard:
     uses: pcdshub/pcds-ci-helpers/.github/workflows/python-standard.yml@master
+    secrets: inherit
     with:
       # The workflow needs to know the package name.  This can be determined
       # automatically if the repository name is the same as the import name.
       package-name: "nabs"
       # Extras that will be installed for both conda/pip:
       testing-extras: ""
       # Extras to be installed only for conda-based testing:
```

### Comparing `nabs-1.5.3/.gitignore` & `nabs-1.5.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/.pre-commit-config.yaml` & `nabs-1.5.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/CONTRIBUTING.rst` & `nabs-1.5.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/LICENSE.md` & `nabs-1.5.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/PKG-INFO` & `nabs-1.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nabs
-Version: 1.5.3
+Version: 1.5.4
 Summary: NABS: Not a beamline scientist. Beamline automatation that should be handled by code, not by people.
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -43,15 +43,15 @@
         into other computer software, distribute, and sublicense such Enhancements or
         derivative works thereof, in binary and source code form.
         
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 # nabs
 Not a Beamline Scientist
```

### Comparing `nabs-1.5.3/conda-recipe/meta.yaml` & `nabs-1.5.4/conda-recipe/meta.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,22 +17,22 @@
 requirements:
   build:
   - python >=3.6
   - setuptools_scm
   - pip
   run:
   - python >=3.6
-  - bluesky >=1.6.5
+  - bluesky >=1.6.5,<1.11
   - numpy
   - ophyd
   - pandas
   - scipy
   - toolz
   run_constrained:
-  - pyqt <5.15.0
+  - pyqt =5
 
 test:
   requires:
   - matplotlib-base
   - pcdsdaq
   - pcdsdevices
   - pytest
```

### Comparing `nabs-1.5.3/docs/Makefile` & `nabs-1.5.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/pre-release-notes.sh` & `nabs-1.5.4/docs/pre-release-notes.sh`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/release_notes.py` & `nabs-1.5.4/docs/release_notes.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/_templates/autosummary/module.rst` & `nabs-1.5.4/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/conf.py` & `nabs-1.5.4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/index.rst` & `nabs-1.5.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/optimize.rst` & `nabs-1.5.4/docs/source/optimize.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/plans.rst` & `nabs-1.5.4/docs/source/plans.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/docs/source/releases.rst` & `nabs-1.5.4/docs/source/releases.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 Release History
 ###############
 
 
+v1.5.4 (2023-07-25)
+===================
+
+Maintenance
+-----------
+- Adjust PyQt pinning to select PyQt5.
+
+Contributors
+------------
+- klauer
+
+
+
 v1.5.3 (2023-04-04)
 ===================
 
 Maintenance
 -----------
 - Fix an issue with the pre-commit config pointing to a missing url mirror.
 - nabs no longer uses Travis CI and has migrated to GitHub Actions for
```

### Comparing `nabs-1.5.3/docs/source/upcoming_release_notes/template-full.rst` & `nabs-1.5.4/docs/source/upcoming_release_notes/template-full.rst`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/callbacks.py` & `nabs-1.5.4/nabs/callbacks.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/optimize.py` & `nabs-1.5.4/nabs/optimize.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/plan_stubs.py` & `nabs-1.5.4/nabs/plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/plans.py` & `nabs-1.5.4/nabs/plans.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/preprocessors.py` & `nabs-1.5.4/nabs/preprocessors.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/simulators.py` & `nabs-1.5.4/nabs/simulators.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/streams.py` & `nabs-1.5.4/nabs/streams.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/conftest.py` & `nabs-1.5.4/nabs/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_callbacks.py` & `nabs-1.5.4/nabs/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_optimize.py` & `nabs-1.5.4/nabs/tests/test_optimize.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_plan_stubs.py` & `nabs-1.5.4/nabs/tests/test_plan_stubs.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_plans.py` & `nabs-1.5.4/nabs/tests/test_plans.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_preprocessors.py` & `nabs-1.5.4/nabs/tests/test_preprocessors.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_simulators.py` & `nabs-1.5.4/nabs/tests/test_simulators.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/tests/test_streams.py` & `nabs-1.5.4/nabs/tests/test_streams.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/utils.py` & `nabs-1.5.4/nabs/utils.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/version.py` & `nabs-1.5.4/nabs/version.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs/visualizations.py` & `nabs-1.5.4/nabs/visualizations.py`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/nabs.egg-info/PKG-INFO` & `nabs-1.5.4/nabs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nabs
-Version: 1.5.3
+Version: 1.5.4
 Summary: NABS: Not a beamline scientist. Beamline automatation that should be handled by code, not by people.
 Author: SLAC National Accelerator Laboratory
 License: Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
         University, through SLAC National Accelerator Laboratory (subject to receipt
         of any required approvals from the U.S. Dept. of Energy). All rights reserved.
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -43,15 +43,15 @@
         into other computer software, distribute, and sublicense such Enhancements or
         derivative works thereof, in binary and source code form.
         
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
 License-File: LICENSE.md
 License-File: AUTHORS.rst
 
 # nabs
 Not a Beamline Scientist
```

### Comparing `nabs-1.5.3/nabs.egg-info/SOURCES.txt` & `nabs-1.5.4/nabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nabs-1.5.3/pyproject.toml` & `nabs-1.5.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 [tool.setuptools.packages.find]
 where = [ ".",]
 include = [ "nabs*",]
 namespaces = false
 
 [tool.setuptools.dynamic.readme]
 file = "README.md"
+content-type = "text/markdown"
 
 [tool.setuptools.dynamic.dependencies]
 file = [ "requirements.txt",]
 
 [tool.setuptools.dynamic.optional-dependencies.test]
 file = "dev-requirements.txt"
```

