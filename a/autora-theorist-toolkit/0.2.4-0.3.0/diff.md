# Comparing `tmp/autora-theorist-toolkit-0.2.4.tar.gz` & `tmp/autora-theorist-toolkit-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-theorist-toolkit-0.2.4.tar", last modified: Mon Jul 24 18:24:03 2023, max compression
+gzip compressed data, was "autora-theorist-toolkit-0.3.0.tar", last modified: Tue Jul 25 18:31:34 2023, max compression
```

## Comparing `autora-theorist-toolkit-0.2.4.tar` & `autora-theorist-toolkit-0.3.0.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/autora-theorist-toolkit.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/Additional Example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/Basic Usage.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/javascripts/mathjax.js
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/docs/quickstart.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.751158 autora-theorist-toolkit-0.2.4/src/autora/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/primitives.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.755158 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/ddm_bms.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hybrid_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    10984 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/symbolic_regression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-24 18:24:03.000000 autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-24 18:24:03.759158 autora-theorist-toolkit-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/test_toolkit.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-24 18:23:47.000000 autora-theorist-toolkit-0.2.4/tests/test_visual.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/autora-theorist-toolkit.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/docs/Additional Example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/docs/Basic Usage.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/docs/quickstart.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/src/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.630573 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/primitives.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/ddm_bms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4294 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hybrid_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/symbolic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7212 2023-07-25 18:31:34.000000 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-25 18:31:34.000000 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 18:31:34.000000 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-25 18:31:34.000000 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 18:31:34.000000 autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:34.634574 autora-theorist-toolkit-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/tests/test_toolkit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-07-25 18:31:19.000000 autora-theorist-toolkit-0.3.0/tests/test_visual.py
```

### Comparing `autora-theorist-toolkit-0.2.4/.github/pull_request_template.md` & `autora-theorist-toolkit-0.3.0/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/.github/workflows/python-publish.yml` & `autora-theorist-toolkit-0.3.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/.gitignore` & `autora-theorist-toolkit-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/.idea/inspectionProfiles/Project_Default.xml` & `autora-theorist-toolkit-0.3.0/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/.pre-commit-config.yaml` & `autora-theorist-toolkit-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/PKG-INFO` & `autora-theorist-toolkit-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.4
+Version: 0.3.0
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.4/README.md` & `autora-theorist-toolkit-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/docs/Additional Example.ipynb` & `autora-theorist-toolkit-0.3.0/docs/Additional Example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/docs/Basic Usage.ipynb` & `autora-theorist-toolkit-0.3.0/docs/Basic Usage.ipynb`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/docs/index.md` & `autora-theorist-toolkit-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/mkdocs/base.yml` & `autora-theorist-toolkit-0.3.0/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/pyproject.toml` & `autora-theorist-toolkit-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/nodes.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/nodes.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/components/primitives.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/components/primitives.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/fitting.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/fitting.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/metrics.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/metrics.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/methods/rules.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/methods/rules.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/bayesian_machine_scientist.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/bayesian_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hierarchical_bayesian_symbolic_regression.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,30 @@
     "log": 10.0,
 }
 
 temperatures_ = [1.04**n for n in range(20)]
 
 
 class HierarchicalBayesianSymbolicRegression:
-    def __init__(self, temperatures=None, prior_dict=None, primitives=None):
+    def __init__(self, temperatures=None, prior_dict=None, primitives=None, seed=0):
+        self.seed = seed
+        np.random.seed(seed)
         self.temperatures = temperatures_ if temperatures is None else temperatures
         self.prior_dict = prior_dict_ if prior_dict is None else prior_dict
         primitives_ = default_primitives if primitives is None else primitives
         self.primitives = [
             primitive
             for primitive in primitives_
             if str(primitive) in list(self.prior_dict.keys())
         ]
         self.theorists = [
-            HierarchicalSymbolicRegressor(primitives=self.primitives)
+            HierarchicalSymbolicRegressor(primitives=self.primitives, seed=self.seed)
             for _ in self.temperatures
         ]
+        self.model_ = self.theorists[-1]
 
     def fit(self, x, y, g, epochs=100, verbose=False):
         n_swaps = 0
         for theorist in self.theorists:
             theorist.load_data(x, y, g)
         for n in tqdm(range(epochs)):
             for i, theorist in enumerate(self.theorists):
```

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hierarchical_symbolic_regressor.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,19 +8,20 @@
 from autora.theorist.toolkit.methods.regression import regression_handler
 from autora.theorist.toolkit.methods.rules import less_than
 from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.models.symbolic_regression import SymbolicRegressor
 
 
 class HierarchicalSymbolicRegressor(SymbolicRegressor):
-    def __init__(self, primitives=None):
-        super().__init__(primitives=primitives)
+    def __init__(self, primitives=None, seed=0):
+        super().__init__(primitives=primitives, seed=seed)
         self.ids = list()
         self.id_parameters = dict()
         self.parameter_cache = Stack()
+        np.random.seed(seed)
 
     def load_data(self, x, y, g):
         if isinstance(x, pd.DataFrame) and isinstance(y, pd.DataFrame):
             dv_variables, iv_variables = x.columns, y.columns
         elif isinstance(x, np.ndarray):
             dv_variables = ["_x" + str(i) + "_" for i in range(x.shape[1])]
             iv_variables = ["_y" + str(i) + "_" for i in range(y.shape[1])]
```

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/hybrid_regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/hybrid_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/memory.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/memory.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/parallel_symbolic_regression.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/symbolic_regression.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/symbolic_regression.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from autora.theorist.toolkit.models.memory import Stack
 from autora.theorist.toolkit.models.tree import Tree
 
 
 class SymbolicRegressor(BaseEstimator):
 
     # TODO: replace tree=None with expression=None once build_tree() is made
-    def __init__(self, tree=None, moves=None, primitives=None, metric=None):
+    def __init__(self, tree=None, moves=None, primitives=None, metric=None, seed=0):
         self.DVs = dict()  # currently unused
         self.IVs = dict()  # currently unused
         self.model_ = Tree() if tree is None else tree
         self.metric = mean_squared_error if metric is None else metric
         self._primitives = default_primitives if primitives is None else primitives
         self._custom_primitives = {
             primitive[0]: primitive[1]
@@ -53,14 +53,15 @@
         )
         self._variables: List[str] = list()
         self._trace: List[float] = []
         self._complete(depth=0)
         self._history = []
         self._visit_list = set()
         self._error = np.inf
+        np.random.seed(seed)
 
     def __repr__(self, N_CHAR_MAX=None):
         if N_CHAR_MAX is None:
             # Symbolic Regressor __repr__ method
             return self.model_.__repr__()
         else:
             # Sci-kit Learn __repr__ method
```

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/models/tree.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/models/tree.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora/theorist/toolkit/utils.py` & `autora-theorist-toolkit-0.3.0/src/autora/theorist/toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/PKG-INFO` & `autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-theorist-toolkit
-Version: 0.2.4
+Version: 0.3.0
 Summary: Toolkit to build algorithms for model recovery
 Author-email: "Joshua T. S. Hewson" <joshua_hewson@brown.edu>
 License: MIT license
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/TheLemonPig/autora-theorist-toolkit
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
```

### Comparing `autora-theorist-toolkit-0.2.4/src/autora_theorist_toolkit.egg-info/SOURCES.txt` & `autora-theorist-toolkit-0.3.0/src/autora_theorist_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/tests/README.md` & `autora-theorist-toolkit-0.3.0/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-theorist-toolkit-0.2.4/tests/test_toolkit.py` & `autora-theorist-toolkit-0.3.0/tests/test_toolkit.py`

 * *Files 22% similar despite different names*

```diff
@@ -77,13 +77,29 @@
     y = 1 + x[:, 0] + x[:, 1]
     y = y.reshape((-1, 1))
     g = np.ones_like(y)
     hbsr = HierarchicalBayesianSymbolicRegression()
     hbsr.fit(x=x, y=y, g=g, epochs=30)
 
 
+def test_hbsr_seed():
+    hbsr1 = HierarchicalBayesianSymbolicRegression(seed=1)
+    hbsr2 = HierarchicalBayesianSymbolicRegression(seed=2)
+    for _ in range(25):
+        hbsr1.theorists[-1].step()
+        hbsr2.theorists[-1].step()
+    assert str(hbsr1.theorists[-1].model_) != str(
+        hbsr2.theorists[-1].model_
+    ), f"{str(hbsr1.theorists[-1].model_)} {str(hbsr2.theorists[-1].model_)}"
+
+
+def test_hbsr_model_():
+    hbsr = HierarchicalBayesianSymbolicRegression()
+    assert hasattr(hbsr, "model_") and hbsr.model_ is not None
+
+
 if __name__ == "__main__":
     test_symbolic_regression_initialization()
     test_bayesian_symbolic_regression_initialization()
     test_parallel_symbolic_regression_initialization()
     test_bayesian_machine_scientist_initialization()
     test_hbsr_multi_x()
```

### Comparing `autora-theorist-toolkit-0.2.4/tests/test_visual.py` & `autora-theorist-toolkit-0.3.0/tests/test_visual.py`

 * *Files identical despite different names*

