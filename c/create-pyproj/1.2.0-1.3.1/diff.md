# Comparing `tmp/create-pyproj-1.2.0.tar.gz` & `tmp/create-pyproj-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "create-pyproj-1.2.0.tar", last modified: Sat Jan 14 18:53:45 2023, max compression
+gzip compressed data, was "create-pyproj-1.3.1.tar", last modified: Tue Jul 25 13:54:29 2023, max compression
```

## Comparing `create-pyproj-1.2.0.tar` & `create-pyproj-1.3.1.tar`

### file list

```diff
@@ -1,66 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.301840 create-pyproj-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1886 2023-01-14 18:53:45.301840 create-pyproj-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1287 2023-01-14 18:53:45.302841 create-pyproj-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.281839 create-pyproj-1.2.0/src/
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-01-14 18:53:37.000000 create-pyproj-1.2.0/src/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.283839 create-pyproj-1.2.0/src/create_pyproj/
--rw-rw-rw-   0 root         (0) root         (0)       43 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.288840 create-pyproj-1.2.0/src/create_pyproj/_config/
--rw-rw-rw-   0 root         (0) root         (0)      133 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/_config/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      645 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/_config/logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)      246 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/_config/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.289840 create-pyproj-1.2.0/src/create_pyproj/code/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/__init__.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.291840 create-pyproj-1.2.0/src/create_pyproj/code/_config/
--rw-rw-rw-   0 root         (0) root         (0)      240 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/_config/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/_config/logger.py
--rw-rw-rw-   0 root         (0) root         (0)      646 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/_config/logging.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1553 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/_config/settings.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/_config/version.py
--rw-rw-rw-   0 root         (0) root         (0)      931 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/main.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.292840 create-pyproj-1.2.0/src/create_pyproj/code/scripts/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/scripts/pre_commit.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/scripts/update_readme.py
--rw-rw-rw-   0 root         (0) root         (0)        4 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/settings.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.293840 create-pyproj-1.2.0/src/create_pyproj/code/test/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       96 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/code/test/test_main.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/createfile.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/figlet.py
--rw-rw-rw-   0 root         (0) root         (0)      587 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/initialise.py
--rw-rw-rw-   0 root         (0) root         (0)     2664 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/main.py
--rw-rw-rw-   0 root         (0) root         (0)      981 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templater.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.278839 create-pyproj-1.2.0/src/create_pyproj/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.295840 create-pyproj-1.2.0/src/create_pyproj/templates/package/
--rw-rw-rw-   0 root         (0) root         (0)     1072 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/package/LICENSE.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/package/MANIFEST.in.tmpl
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/package/pyproject.toml.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1175 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/package/setup.cfg.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.299840 create-pyproj-1.2.0/src/create_pyproj/templates/project/
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/.env.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      162 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/.flake8.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/.gitignore.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/.gitlab-ci.yml.tmpl
--rw-rw-rw-   0 root         (0) root         (0)    11903 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/.style.yapf.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      518 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/Pipfile.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     3015 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/README.md.tmpl
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/VERSION.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/project/pytest.ini.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.300840 create-pyproj-1.2.0/src/create_pyproj/templates/vscode/
--rw-rw-rw-   0 root         (0) root         (0)      245 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/vscode/extensions.json.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/vscode/launch.json.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      659 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/src/create_pyproj/templates/vscode/settings.json.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.286839 create-pyproj-1.2.0/src/create_pyproj.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1886 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2026 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       43 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-01-14 18:53:45.000000 create-pyproj-1.2.0/src/create_pyproj.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-01-14 18:53:45.301840 create-pyproj-1.2.0/test/
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-01-14 18:53:20.000000 create-pyproj-1.2.0/test/test_main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.791689 create-pyproj-1.3.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-25 13:54:29.791689 create-pyproj-1.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-25 13:54:29.791689 create-pyproj-1.3.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.774688 create-pyproj-1.3.1/src/
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.776688 create-pyproj-1.3.1/src/create_pyproj/
+-rw-rw-rw-   0 root         (0) root         (0)       43 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.780688 create-pyproj-1.3.1/src/create_pyproj/_config/
+-rw-rw-rw-   0 root         (0) root         (0)      133 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/_config/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      645 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/_config/logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      246 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/_config/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.781688 create-pyproj-1.3.1/src/create_pyproj/code/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/__init__.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.783688 create-pyproj-1.3.1/src/create_pyproj/code/_config/
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/_config/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1686 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/_config/logger.py
+-rw-rw-rw-   0 root         (0) root         (0)      646 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/_config/logging.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1518 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/_config/settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/_config/version.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/main.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.783688 create-pyproj-1.3.1/src/create_pyproj/code/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/scripts/pre_commit.py
+-rw-rw-rw-   0 root         (0) root         (0)        4 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/settings.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.785688 create-pyproj-1.3.1/src/create_pyproj/code/test/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/test/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/test/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/code/test/test_main.py
+-rw-rw-rw-   0 root         (0) root         (0)     2818 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/createfile.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/figlet.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/initialise.py
+-rw-rw-rw-   0 root         (0) root         (0)     2492 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/main.py
+-rw-rw-rw-   0 root         (0) root         (0)      930 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templater.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.772688 create-pyproj-1.3.1/src/create_pyproj/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.786689 create-pyproj-1.3.1/src/create_pyproj/templates/package/
+-rw-rw-rw-   0 root         (0) root         (0)     1072 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/package/LICENSE.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/package/MANIFEST.in.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1107 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/package/pyproject.toml.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.789689 create-pyproj-1.3.1/src/create_pyproj/templates/project/
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/.env.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/.flake8.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/.gitignore.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      390 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/.gitlab-ci.yml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/.pre-commit-config.yaml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/Pipfile.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     3015 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/README.md.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/project/VERSION.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.790689 create-pyproj-1.3.1/src/create_pyproj/templates/vscode/
+-rw-rw-rw-   0 root         (0) root         (0)      288 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/vscode/extensions.json.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/vscode/launch.json.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/src/create_pyproj/templates/vscode/settings.json.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.778688 create-pyproj-1.3.1/src/create_pyproj.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-07-25 13:54:29.000000 create-pyproj-1.3.1/src/create_pyproj.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-07-25 13:54:29.000000 create-pyproj-1.3.1/src/create_pyproj.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 13:54:29.000000 create-pyproj-1.3.1/src/create_pyproj.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-25 13:54:29.000000 create-pyproj-1.3.1/src/create_pyproj.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 13:54:29.790689 create-pyproj-1.3.1/test/
+-rw-rw-rw-   0 root         (0) root         (0)      833 2023-07-25 13:54:16.000000 create-pyproj-1.3.1/test/test_main.py
```

### Comparing `create-pyproj-1.2.0/LICENSE` & `create-pyproj-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/_config/logger.py` & `create-pyproj-1.3.1/src/create_pyproj/_config/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,41 @@
 import logging
 from logging.config import dictConfig
 from pathlib import Path
 
 import yaml
 
 DIR = Path(__file__).parent.absolute()
-LOGPATH = DIR.parent.parent.parent / 'logs'
+LOGPATH = DIR.parent.parent.parent / "logs"
 
 
 def removeExistingLogs():
-    """
-    Remove old logs, so one clean log per run.
-    """
+    """Remove old logs, so one clean log per run."""
     try:
-        Path(LOGPATH / 'debug.log').unlink(missing_ok=True)
-        Path(LOGPATH / 'debug.log.1').unlink(missing_ok=True)
-        Path(LOGPATH / 'main.log').unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log").unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log.1").unlink(missing_ok=True)
+        Path(LOGPATH / "main.log").unlink(missing_ok=True)
     except Exception as e:
         print(e)
 
 
 def configureLogging(clearLogs: bool = False):
     """."""
     if clearLogs:
         removeExistingLogs()
 
     Path(LOGPATH).mkdir(exist_ok=True, parents=True)
-    mainfilename = LOGPATH / 'main.log'
-    debugfilename = LOGPATH / 'debug.log'
+    mainfilename = LOGPATH / "main.log"
+    debugfilename = LOGPATH / "debug.log"
 
-    with open(DIR / 'logging.yaml', 'r') as f:
+    with open(DIR / "logging.yaml", "r") as f:
         log_cfg = yaml.full_load(f)
 
-    log_cfg['handlers']['file_handler']['filename'] = mainfilename
-    log_cfg['handlers']['rotating_handler']['filename'] = debugfilename
+    log_cfg["handlers"]["file_handler"]["filename"] = mainfilename
+    log_cfg["handlers"]["rotating_handler"]["filename"] = debugfilename
 
     dictConfig(log_cfg)
 
     # Set ERROR level logging on verbose modules
     modules = []
     for module in modules:
         logging.getLogger(module).setLevel(logging.ERROR)
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/_config/logging.yaml` & `create-pyproj-1.3.1/src/create_pyproj/_config/logging.yaml`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/code/_config/logger.py` & `create-pyproj-1.3.1/src/create_pyproj/code/_config/logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,58 @@
 # -*- coding: utf-8 -*-
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import logging
 from logging import config
 from pathlib import Path
 
 import yaml
 
 DIR = Path(__file__).parent.absolute()
-LOGPATH = DIR.parent.parent / 'logs'
+LOGPATH = DIR.parent.parent / "logs"
 
 
 def removeExistingLogs():
-    """
-    Remove old logs, so one clean log per run.
-    """
+    """Remove old logs, so one clean log per run."""
     try:
-        Path(LOGPATH / 'debug.log').unlink(missing_ok=True)
-        Path(LOGPATH / 'debug.log.1').unlink(missing_ok=True)
-        Path(LOGPATH / 'main.log').unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log").unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log.1").unlink(missing_ok=True)
+        Path(LOGPATH / "main.log").unlink(missing_ok=True)
     except Exception as e:
         print(e)
 
 
 def cycleLogRuns(days: int = 10):
-    """
-    Save the old logs by date, keep a specificed number of runs and delte the rest.
+    """Save the old logs by date, keep a specificed number of runs and delte the rest.
+
     - Delete logs older than days
     - Save last log as a new date/run log
     - create new log
     """
     try:
-        Path(LOGPATH / 'debug.log').unlink(missing_ok=True)
-        Path(LOGPATH / 'debug.log.1').unlink(missing_ok=True)
-        Path(LOGPATH / 'main.log').unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log").unlink(missing_ok=True)
+        Path(LOGPATH / "debug.log.1").unlink(missing_ok=True)
+        Path(LOGPATH / "main.log").unlink(missing_ok=True)
     except Exception as e:
         print(e)
 
 
 def configureLogging(clearLogs: bool = False):
     """."""
     if clearLogs:
         removeExistingLogs()
 
     Path(LOGPATH).mkdir(exist_ok=True, parents=True)
-    mainfilename = LOGPATH / 'main.log'
-    debugfilename = LOGPATH / 'debug.log'
+    mainfilename = LOGPATH / "main.log"
+    debugfilename = LOGPATH / "debug.log"
 
-    with open(DIR / 'logging.yaml', 'r') as f:
+    with open(DIR / "logging.yaml", "r") as f:
         log_cfg = yaml.full_load(f)
 
-    log_cfg['handlers']['file_handler']['filename'] = mainfilename
-    log_cfg['handlers']['rotating_handler']['filename'] = debugfilename
+    log_cfg["handlers"]["file_handler"]["filename"] = mainfilename
+    log_cfg["handlers"]["rotating_handler"]["filename"] = debugfilename
 
     config.dictConfig(log_cfg)
 
     # Set ERROR level logging on verbose modules
-    modules = ['botocore', 'urllib3', 'googleapiclient', 'numba']
+    modules = ["botocore", "urllib3", "googleapiclient", "numba"]
     for module in modules:
         logging.getLogger(module).setLevel(logging.ERROR)
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/code/_config/logging.yaml` & `create-pyproj-1.3.1/src/create_pyproj/code/_config/logging.yaml`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/code/_config/settings.py` & `create-pyproj-1.3.1/src/create_pyproj/code/_config/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 # -*- coding: utf-8 -*-
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 from pathlib import Path
 
 import yaml
 from pydantic import BaseSettings as PyBaseSettings
 
 DIR = Path(__file__).parent.parent
 SETTINGS_PATH = Path(DIR).absolute()
 
 
-def saveSettings(settings: dict,
-                 settings_file_name: str = 'settings',
-                 settings_path: Path = SETTINGS_PATH,
-                 sort_keys: bool = False) -> None:
+def saveSettings(
+    settings: dict,
+    settings_file_name: str = "settings",
+    settings_path: Path = SETTINGS_PATH,
+    sort_keys: bool = False,
+) -> None:
     settings_path.mkdir(exist_ok=True, parents=True)
-    with open(settings_path / f'{settings_file_name}.yaml', 'w') as f:
+    with open(settings_path / f"{settings_file_name}.yaml", "w") as f:
         yaml.dump(settings, f, sort_keys=sort_keys)
 
 
-def loadSettings(settings_file_name: str = 'settings', settings_path: Path = SETTINGS_PATH) -> dict:
-    if (not (settings_path / f'{settings_file_name}.yaml').exists()):
+def loadSettings(
+    settings_file_name: str = "settings", settings_path: Path = SETTINGS_PATH
+) -> dict:
+    if not (settings_path / f"{settings_file_name}.yaml").exists():
         saveSettings({})
-    with open(settings_path / f'{settings_file_name}.yaml', 'r') as f:
+    with open(settings_path / f"{settings_file_name}.yaml", "r") as f:
         settings = yaml.full_load(f)
     return settings
 
 
 class BaseSettings(PyBaseSettings):
-    """
-    An extension of Pydantic with a custom yaml loader
+    """An extension of Pydantic with a custom yaml loader.
 
     https://pydantic-docs.helpmanual.io/usage/settings/#adding-sources
 
     Args:
         PyBaseSettings (BaseSettings): Pydantic basesettings
     """
+
     class Config:
-        env_file_encoding = 'utf-8'
+        env_file_encoding = "utf-8"
 
         @classmethod
         def customise_sources(
             cls,
             init_settings,
             env_settings,
             file_secret_settings,
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/code/_config/version.py` & `create-pyproj-1.3.1/src/create_pyproj/code/_config/version.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # -*- coding: utf-8 -*-
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import configparser
 from pathlib import Path
 
 DIR = Path(__file__).parent.absolute()
 
 
 def getVersionFromSetup():
     """Get version from setup.cfg file."""
     config = configparser.ConfigParser()
-    config.read(DIR.parent.parent / 'setup.cfg')
-    return config.get('metadata', 'version')
+    config.read(DIR.parent.parent / "setup.cfg")
+    return config.get("metadata", "version")
 
 
 def getVersion():
     """Get version from VERSION file."""
-    with open(DIR.parent.parent / 'VERSION', 'r') as f:
+    with open(DIR.parent.parent / "VERSION", "r") as f:
         VERSION = f.read().strip()
     return VERSION
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/code/main.py.tmpl` & `create-pyproj-1.3.1/src/create_pyproj/code/main.py.tmpl`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/createfile.py` & `create-pyproj-1.3.1/src/create_pyproj/createfile.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import logging
 import shutil
 from pathlib import Path
 
 from .figlet import figletise
 from .templater import writeTemplate
 
 DIR = Path(__file__).parent.absolute()
 logger = logging.getLogger(__name__)
 
 
 def copyTemplates(projectname: str, cli: bool):
-    """
-    Copy templates into folder structure.
+    """Copy templates into folder structure.
 
     Args:
         projectname (str): The project name.
-        cli (bool, optional): True if this is intended as a cli application. Defaults to False.
+        cli (bool, optional): True if this is intended as a cli application.
+            Defaults to False.
     """
     # Set the path for the main code repo
     PROJECT_ROOT = Path.cwd() / projectname
-    PROJECT_PATH = PROJECT_ROOT / 'src' / projectname.replace('-', '_')
+    PROJECT_PATH = PROJECT_ROOT / "src" / projectname.replace("-", "_")
     PROJECT_PATH.mkdir(exist_ok=True, parents=True)
-    (PROJECT_PATH / '__init__.py').touch(exist_ok=True)
-    for item in (DIR / 'code').iterdir():
-        if item.stem == 'scripts':
+    (PROJECT_PATH / "__init__.py").touch(exist_ok=True)
+    for item in (DIR / "code").iterdir():
+        if item.stem == "scripts":
             shutil.copytree(item, PROJECT_ROOT / item.stem)
-        elif item.stem == 'test':
+        elif item.stem == "test":
             shutil.copytree(item, PROJECT_ROOT / item.stem)
-        elif item.stem == '_config':
-            shutil.copytree(item, PROJECT_ROOT / 'src' / item.stem)
-        elif item.stem == 'main.py':
-            data = {'projectname': projectname, 'cli': cli}
-            writeTemplate('main.py', PROJECT_ROOT / 'src', data=data, templatepath=DIR / 'code')
-        elif item.stem == '__init__.py':
-            data = {'projectname': projectname, 'cli': cli}
-            writeTemplate('__init__.py',
-                          PROJECT_ROOT / 'src',
-                          data=data,
-                          templatepath=DIR / 'code')
+        elif item.stem == "_config":
+            shutil.copytree(item, PROJECT_ROOT / "src" / item.stem)
+        elif item.stem == "main.py":
+            data = {"projectname": projectname, "cli": cli}
+            writeTemplate(
+                "main.py", PROJECT_ROOT / "src", data=data, templatepath=DIR / "code"
+            )
+        elif item.stem == "__init__.py":
+            data = {"projectname": projectname, "cli": cli}
+            writeTemplate(
+                "__init__.py",
+                PROJECT_ROOT / "src",
+                data=data,
+                templatepath=DIR / "code",
+            )
         else:
             if not item.is_dir():
-                shutil.copy(item, PROJECT_ROOT / 'src' / item.name)
+                shutil.copy(item, PROJECT_ROOT / "src" / item.name)
 
 
-def createFiles(projectname: str, cli: bool, python_version: str):
+def createFiles(
+    projectname: str,
+    cli: bool,
+    python_version: str,
+    author: str = "author",
+    author_email: str = "author@email.com",
+    description: str = "description",
+):
     PROJECT_ROOT = Path.cwd() / projectname
     data = {
-        'projectname': projectname,
-        'python_version': python_version,
-        'figleted': figletise(projectname),
-        'cli': cli,
-        'author': None,
-        'author_email': None,
-        'description': None,
-        'hashes': '##'
+        "projectname": projectname,
+        "python_version": python_version,
+        "figleted": figletise(projectname),
+        "cli": cli,
+        "author": author,
+        "author_email": author_email,
+        "description": description,
+        "hashes": "##",
     }
 
     project = [
-        '.env',
-        '.flake8',
-        '.gitignore',
-        '.gitlab-ci.yml',
-        '.style.yapf',
-        'README.md',
-        'Pipfile',
-        'VERSION',
-        'pytest.ini',
+        ".env",
+        ".flake8",
+        ".gitignore",
+        ".gitlab-ci.yml",
+        ".pre-commit-config.yaml",
+        "Pipfile",
+        "README.md",
+        "VERSION",
+        "LICENSE",
+        "pyproject.toml",
+        "MANIFEST.in",
     ]
 
     for tmpl in project:
-        writeTemplate(tmpl, PROJECT_ROOT, data=data, templatepath='project')
+        writeTemplate(tmpl, PROJECT_ROOT, data=data, templatepath="project")
 
     vscode = [
-        'launch.json',
-        'settings.json',
-        'extensions.json',
+        "launch.json",
+        "settings.json",
+        "extensions.json",
     ]
     for tmpl in vscode:
-        writeTemplate(tmpl, PROJECT_ROOT / '.vscode', data=data, templatepath='vscode')
-
-    package = [
-        'LICENSE',
-        'setup.cfg',
-        'pyproject.toml',
-        'MANIFEST.in',
-    ]
-    for tmpl in package:
-        writeTemplate(tmpl, PROJECT_ROOT, data=data, templatepath='package')
+        writeTemplate(tmpl, PROJECT_ROOT / ".vscode", data=data, templatepath="vscode")
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/initialise.py` & `create-pyproj-1.3.1/src/create_pyproj/initialise.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import logging
 import os
 from pathlib import Path
 
 CWD = Path.cwd()
 logger = logging.getLogger(__name__)
 
 
 def initialise(projectname: str, no_init: bool, no_install: bool) -> None:
     PROJDIR = CWD.absolute() / projectname
     os.chdir(PROJDIR)
 
     # Whether to install in Pipenv
     if not no_install:
-        os.system('pipenv install -d')
+        os.system("pipenv install -d")
 
     # Whether to init the git repo
     if not no_init:
-        git_init = ['git init --initial-branch=main', 'git add -A', 'git commit -m "first commit"']
+        git_init = [
+            "git init --initial-branch=main",
+            "git add -A",
+            'git commit -m "first commit"',
+        ]
         for cmd in git_init:
             os.system(cmd)
+
+    # Install pre-commit hooks
+    os.system("pre-commit install")
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/main.py` & `create-pyproj-1.3.1/src/create_pyproj/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,74 +1,89 @@
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import argparse
 import logging
 import textwrap
 
 from ._config import configureLogging
 from .createfile import copyTemplates, createFiles
 from .figlet import figletise
 from .initialise import initialise
 
 configureLogging()
 logger = logging.getLogger(__name__)
 
 
 def create_pyproj(args: argparse.Namespace):
-    logger.info(f'Making new project...{figletise(args.projectname)}')
+    logger.info(f"Making new project...{figletise(args.projectname)}")
 
     try:
         copyTemplates(args.projectname, args.cli)
         createFiles(args.projectname, args.cli, args.python_version)
         initialise(args.projectname, args.no_init, args.no_install)
-        logger.info(f'Install complete!\ncd into {args.projectname} and get developing...')
+        logger.info(
+            f"Install complete!\ncd into {args.projectname} and get developing..."
+        )
     except FileExistsError:
         logger.error(
-            'The destination project already exists, please remove or choose another name.')
+            """The destination project already exists,
+            please remove or choose another name."""
+        )
 
 
 def main():
-    parser = argparse.ArgumentParser(prog='create-pyproj',
-                                     formatter_class=argparse.RawDescriptionHelpFormatter,
-                                     description=textwrap.dedent('''\
+    parser = argparse.ArgumentParser(
+        prog="create-pyproj",
+        formatter_class=argparse.RawDescriptionHelpFormatter,
+        description=textwrap.dedent(
+            """\
     Create a new python skeleton project.
     --------------------------------
     The project has a number of development tools
     and convenince functions to get you started quickly!
 
     usage:
     create-pyproj <projectname> [options]
 
-    The project structure will be copied to a folder ./<projectname>, the modules installed with Pipenv and a git repo initiated.
-    '''))
-    parser.add_argument('projectname', help='The name of the project you want to start.')
-    parser.add_argument('--python_version',
-                        action='store',
-                        type=str,
-                        default="3.10",
-                        choices=['3.8', '3.9', '3.10'],
-                        help='Select the python version. Defaults to 3.10.')
-    parser.add_argument('--cli',
-                        action='store_const',
-                        const=True,
-                        default=False,
-                        help='Select this option if this is intended to run on the command line.')
-    parser.add_argument('--no-init',
-                        action='store_const',
-                        const=True,
-                        default=False,
-                        help='Select this option to not initialise a git repo.')
-    parser.add_argument('--no-install',
-                        action='store_const',
-                        const=True,
-                        default=False,
-                        help='Select this option to not install the packages.')
+    The project structure will be copied to a folder ./<projectname>,
+    the modules installed with Pipenv and a git repo initiated.
+    """
+        ),
+    )
+    parser.add_argument(
+        "projectname", help="The name of the project you want to start."
+    )
+    parser.add_argument(
+        "--python_version",
+        action="store",
+        type=str,
+        default="3.10",
+        choices=["3.8", "3.9", "3.10"],
+        help="Select the python version. Defaults to 3.10.",
+    )
+    parser.add_argument(
+        "--cli",
+        action="store_const",
+        const=True,
+        default=False,
+        help="Select this option if this is intended to run on the command line.",
+    )
+    parser.add_argument(
+        "--no-init",
+        action="store_const",
+        const=True,
+        default=False,
+        help="Select this option to not initialise a git repo.",
+    )
+    parser.add_argument(
+        "--no-install",
+        action="store_const",
+        const=True,
+        default=False,
+        help="Select this option to not install the packages.",
+    )
 
     args = parser.parse_args()
     create_pyproj(args)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/templater.py` & `create-pyproj-1.3.1/src/create_pyproj/templater.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,34 @@
-"""
-Module Description.
-
-
-"""
+"""Module Description."""
 import logging
 from pathlib import Path
 
 from mako.template import Template
 
 DIR = Path(__file__).parent.absolute()
 
 logger = logging.getLogger(__name__)
 
 
-def writeTemplate(filename: str,
-                  outputpath: Path,
-                  data: dict = {},
-                  templatepath: Path = None,
-                  templateroot: Path = DIR / 'templates') -> None:
-    """
-    [summary]
-
-    [extended_summary]
+def writeTemplate(
+    filename: str,
+    outputpath: Path,
+    data: dict = {},
+    templatepath: Path = None,
+    templateroot: Path = DIR / "templates",
+) -> None:
+    """Write a template file to the outputpath.
 
     Args:
         filename (str): [description]
         data (dict, optional): [description]. Defaults to {}.
         outputpath (Path, optional): [description]. Defaults to None.
     """
     if templatepath is None:
         path = templateroot
     else:
         path = templateroot / templatepath
 
-    template = str(path / f'{filename}.tmpl')
-    mytemplate = Template(filename=template, output_encoding='utf-8')
+    template = str(path / f"{filename}.tmpl")
+    mytemplate = Template(filename=template, output_encoding="utf-8")
     outputpath.mkdir(exist_ok=True, parents=True)
     (outputpath / filename).write_bytes(mytemplate.render(**data))
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj/templates/package/LICENSE.tmpl` & `create-pyproj-1.3.1/src/create_pyproj/templates/package/LICENSE.tmpl`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/templates/project/README.md.tmpl` & `create-pyproj-1.3.1/src/create_pyproj/templates/project/README.md.tmpl`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/templates/vscode/launch.json.tmpl` & `create-pyproj-1.3.1/src/create_pyproj/templates/vscode/launch.json.tmpl`

 * *Files identical despite different names*

### Comparing `create-pyproj-1.2.0/src/create_pyproj/templates/vscode/settings.json.tmpl` & `create-pyproj-1.3.1/src/create_pyproj/templates/vscode/settings.json.tmpl`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 {
-    "autoDocstring.docstringFormat": "google",
-    "isort.args": [
-        "--profile",
-        "hug"
-    ],
-    "isort.importStrategy": "fromEnvironment",
-    "python.formatting.provider": "yapf",
-    "python.linting.flake8Enabled": true,
-    "python.linting.pylintEnabled": false,
-    "python.testing.pytestArgs": [
-      "-c", "./pytest.ini"
-    ],
-    "python.testing.pytestEnabled": true,
-    "python.testing.unittestEnabled": false,
-    "runItOn": {
-        "commands": [
-          {
-            "match": "\\.py$",
-            "isAsync": true,
-            "isShellCommand": false,
-            "cmd": "testing.runAll"
-          },
-        ],
-      },
+  "autoDocstring.docstringFormat": "google",
+  "python.formatting.provider": "black",
+  "python.linting.flake8Enabled": true,
+  "files.autoSave": "afterDelay",
+  "[python]": {
+    "editor.defaultFormatter": "ms-python.black-formatter",
+    "editor.formatOnSave": true,
+    "editor.codeActionsOnSave": {
+      "source.organizeImports": true
+    }
+  },
+  "isort.args": ["--profile", "black"],
+  "python.analysis.inlayHints.functionReturnTypes": true,
+  // "python.analysis.typeCheckingMode": "strict",
+  "rewrap.wrappingColumn": 88,
+  "editor.rulers": [
+    88
+  ],
+  "python.testing.pytestArgs": [
+    "test"
+  ],
+  "python.testing.unittestEnabled": false,
+  "python.testing.pytestEnabled": true,
 }
```

### Comparing `create-pyproj-1.2.0/src/create_pyproj.egg-info/SOURCES.txt` & `create-pyproj-1.3.1/src/create_pyproj.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 LICENSE
 MANIFEST.in
+VERSION
 pyproject.toml
-setup.cfg
 src/__init__.py
 src/create_pyproj/__init__.py
 src/create_pyproj/createfile.py
 src/create_pyproj/figlet.py
 src/create_pyproj/initialise.py
 src/create_pyproj/main.py
 src/create_pyproj/templater.py
 src/create_pyproj.egg-info/PKG-INFO
 src/create_pyproj.egg-info/SOURCES.txt
 src/create_pyproj.egg-info/dependency_links.txt
-src/create_pyproj.egg-info/entry_points.txt
-src/create_pyproj.egg-info/requires.txt
 src/create_pyproj.egg-info/top_level.txt
 src/create_pyproj/_config/__init__.py
 src/create_pyproj/_config/logger.py
 src/create_pyproj/_config/logging.yaml
 src/create_pyproj/_config/version.py
 src/create_pyproj/code/__init__.py.tmpl
 src/create_pyproj/code/main.py.tmpl
@@ -25,27 +23,25 @@
 src/create_pyproj/code/_config/__init__.py
 src/create_pyproj/code/_config/logger.py
 src/create_pyproj/code/_config/logging.yaml
 src/create_pyproj/code/_config/settings.py
 src/create_pyproj/code/_config/version.py
 src/create_pyproj/code/scripts/__init__.py
 src/create_pyproj/code/scripts/pre_commit.py
-src/create_pyproj/code/scripts/update_readme.py
 src/create_pyproj/code/test/__init__.py
+src/create_pyproj/code/test/conftest.py
 src/create_pyproj/code/test/test_main.py
 src/create_pyproj/templates/package/LICENSE.tmpl
 src/create_pyproj/templates/package/MANIFEST.in.tmpl
 src/create_pyproj/templates/package/pyproject.toml.tmpl
-src/create_pyproj/templates/package/setup.cfg.tmpl
 src/create_pyproj/templates/project/.env.tmpl
 src/create_pyproj/templates/project/.flake8.tmpl
 src/create_pyproj/templates/project/.gitignore.tmpl
 src/create_pyproj/templates/project/.gitlab-ci.yml.tmpl
-src/create_pyproj/templates/project/.style.yapf.tmpl
+src/create_pyproj/templates/project/.pre-commit-config.yaml.tmpl
 src/create_pyproj/templates/project/Pipfile.tmpl
 src/create_pyproj/templates/project/README.md.tmpl
 src/create_pyproj/templates/project/VERSION.tmpl
-src/create_pyproj/templates/project/pytest.ini.tmpl
 src/create_pyproj/templates/vscode/extensions.json.tmpl
 src/create_pyproj/templates/vscode/launch.json.tmpl
 src/create_pyproj/templates/vscode/settings.json.tmpl
 test/test_main.py
```

