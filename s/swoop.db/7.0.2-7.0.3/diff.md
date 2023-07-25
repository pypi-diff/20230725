# Comparing `tmp/swoop.db-7.0.2.tar.gz` & `tmp/swoop.db-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-7.0.2.tar", last modified: Wed Jul 12 17:06:22 2023, max compression
+gzip compressed data, was "swoop.db-7.0.3.tar", last modified: Tue Jul 25 17:51:45 2023, max compression
```

## Comparing `swoop.db-7.0.2.tar` & `swoop.db-7.0.3.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.286375 swoop.db-7.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.270374 swoop.db-7.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.278375 swoop.db-7.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.github/workflows/publish-image.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-12 17:06:03.000000 swoop.db-7.0.2/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-12 17:06:03.000000 swoop.db-7.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-12 17:06:03.000000 swoop.db-7.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-12 17:06:03.000000 swoop.db-7.0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-12 17:06:03.000000 swoop.db-7.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-12 17:06:22.286375 swoop.db-7.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-12 17:06:03.000000 swoop.db-7.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-12 17:06:03.000000 swoop.db-7.0.2/RELEASE.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.278375 swoop.db-7.0.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-12 17:06:03.000000 swoop.db-7.0.2/bin/get-max-migration-version.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-12 17:06:03.000000 swoop.db-7.0.2/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-12 17:06:03.000000 swoop.db-7.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-12 17:06:03.000000 swoop.db-7.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-12 17:06:22.286375 swoop.db-7.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.270374 swoop.db-7.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.270374 swoop.db-7.0.2/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.278375 swoop.db-7.0.2/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.278375 swoop.db-7.0.2/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.282375 swoop.db-7.0.2/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00001_version.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00002_cache_func.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00002_cache_func.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00003_remove_items.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00004_update_thread.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00004_update_thread.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00005_handler_type.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00005_handler_type.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00006_workflow_constraint.down.sql
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00006_workflow_constraint.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-12 17:06:03.000000 swoop.db-7.0.2/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.278375 swoop.db-7.0.2/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-12 17:06:22.000000 swoop.db-7.0.2/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.282375 swoop.db-7.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.270374 swoop.db-7.0.2/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.282375 swoop.db-7.0.2/tests/fixtures/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/0_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/1_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/2_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/2_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/6_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/6_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/7_base_01.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/7_result.sql
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/fixtures/migrations/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:06:22.286375 swoop.db-7.0.2/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/pgtap/test_find_cached_action_for_payload.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/pgtap/test_uuid_v7.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-12 17:06:03.000000 swoop.db-7.0.2/tests/test_migrations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.545848 swoop.db-7.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-25 17:51:18.000000 swoop.db-7.0.3/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-07-25 17:51:18.000000 swoop.db-7.0.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-25 17:51:18.000000 swoop.db-7.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-07-25 17:51:18.000000 swoop.db-7.0.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-25 17:51:18.000000 swoop.db-7.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-25 17:51:45.557848 swoop.db-7.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-25 17:51:18.000000 swoop.db-7.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-07-25 17:51:18.000000 swoop.db-7.0.3/RELEASE.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2870 2023-07-25 17:51:18.000000 swoop.db-7.0.3/bin/db-initialization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       92 2023-07-25 17:51:18.000000 swoop.db-7.0.3/bin/get-max-migration-version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 17:51:18.000000 swoop.db-7.0.3/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-25 17:51:18.000000 swoop.db-7.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-25 17:51:18.000000 swoop.db-7.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 17:51:45.557848 swoop.db-7.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.541848 swoop.db-7.0.3/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.553848 swoop.db-7.0.3/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00001_version.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00003_remove_items.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00005_handler_type.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00005_handler_type.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00006_workflow_constraint.down.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00006_workflow_constraint.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/migrations/00007_change-uuid-formats.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16734 2023-07-25 17:51:18.000000 swoop.db-7.0.3/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.549848 swoop.db-7.0.3/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 17:51:45.000000 swoop.db-7.0.3/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.553848 swoop.db-7.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.545848 swoop.db-7.0.3/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/tests/fixtures/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/0_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4673 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/1_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/2_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/2_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/6_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/6_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/7_base_01.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/7_result.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/fixtures/migrations/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 17:51:45.557848 swoop.db-7.0.3/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_find_cached_action_for_payload.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/pgtap/test_uuid_v7.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-07-25 17:51:18.000000 swoop.db-7.0.3/tests/test_migrations.py
```

### Comparing `swoop.db-7.0.2/.env` & `swoop.db-7.0.3/.env`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.github/workflows/publish-image.yml` & `swoop.db-7.0.3/.github/workflows/publish-image.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.github/workflows/python-publish.yml` & `swoop.db-7.0.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.github/workflows/python-test.yml` & `swoop.db-7.0.3/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.github/workflows/snyk-scan.yml` & `swoop.db-7.0.3/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.gitignore` & `swoop.db-7.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.pre-commit-config.yaml` & `swoop.db-7.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/.snyk` & `swoop.db-7.0.3/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/CHANGELOG.md` & `swoop.db-7.0.3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/CONTRIBUTING.md` & `swoop.db-7.0.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/Dockerfile` & `swoop.db-7.0.3/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -29,7 +29,11 @@
 
 ENV PGDATABASE "${PGDATABASE:-swoop}"
 ENV PGUSER "${PGUSER:-postgres}"
 
 # copy the python venv into this output image and add it's bin to the path
 COPY --from=APP /opt/swoop/db/swoop-db-venv /opt/swoop/db/swoop-db-venv
 ENV PATH=/opt/swoop/db/swoop-db-venv/bin:$PATH
+
+RUN mkdir -p /opt/swoop/db/scripts
+COPY bin/db-initialization.py /opt/swoop/db/scripts/db-initialization.py
+ENV PATH=/opt/swoop/db/scripts:$PATH
```

### Comparing `swoop.db-7.0.2/LICENSE` & `swoop.db-7.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/PKG-INFO` & `swoop.db-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.2
+Version: 7.0.3
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.2/README.md` & `swoop.db-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/RELEASE.md` & `swoop.db-7.0.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/docker-compose.yml` & `swoop.db-7.0.3/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/pyproject.toml` & `swoop.db-7.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/cli.py` & `swoop.db-7.0.3/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/fixtures/base_01.sql` & `swoop.db-7.0.3/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00002_cache_func.down.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.down.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00002_cache_func.up.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00002_cache_func.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00004_update_thread.down.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.down.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00004_update_thread.up.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00004_update_thread.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/migrations/00007_change-uuid-formats.up.sql` & `swoop.db-7.0.3/src/swoop/db/migrations/00007_change-uuid-formats.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop/db/schema.sql` & `swoop.db-7.0.3/src/swoop/db/schema.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-7.0.3/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 7.0.2
+Version: 7.0.3
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-7.0.2/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-7.0.3/src/swoop.db.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 docker-compose.yml
 pyproject.toml
 requirements.txt
 .github/workflows/publish-image.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 .github/workflows/snyk-scan.yml
+bin/db-initialization.py
 bin/get-max-migration-version.py
 src/swoop.db.egg-info/PKG-INFO
 src/swoop.db.egg-info/SOURCES.txt
 src/swoop.db.egg-info/dependency_links.txt
 src/swoop.db.egg-info/entry_points.txt
 src/swoop.db.egg-info/requires.txt
 src/swoop.db.egg-info/top_level.txt
```

### Comparing `swoop.db-7.0.2/tests/conftest.py` & `swoop.db-7.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/0_base_01.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/0_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/1_result.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/1_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/2_base_01.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/2_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/2_result.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/2_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/6_base_01.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/6_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/6_result.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/6_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/7_base_01.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/7_base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/7_result.sql` & `swoop.db-7.0.3/tests/fixtures/migrations/7_result.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/fixtures/migrations/README.md` & `swoop.db-7.0.3/tests/fixtures/migrations/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/pgtap/test_action.sql` & `swoop.db-7.0.3/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/pgtap/test_find_cached_action_for_payload.sql` & `swoop.db-7.0.3/tests/pgtap/test_find_cached_action_for_payload.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/pgtap/test_limit-locking.sql` & `swoop.db-7.0.3/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/pgtap/test_uuid_v7.sql` & `swoop.db-7.0.3/tests/pgtap/test_uuid_v7.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/test_database.py` & `swoop.db-7.0.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `swoop.db-7.0.2/tests/test_migrations.py` & `swoop.db-7.0.3/tests/test_migrations.py`

 * *Files identical despite different names*

