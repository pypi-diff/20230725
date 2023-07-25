# Comparing `tmp/lamindb_setup-0.49.0.tar.gz` & `tmp/lamindb_setup-0.49.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.49.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.49.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.49.0.tar` & `lamindb_setup-0.49.1.tar`

### file list

```diff
@@ -1,101 +1,105 @@
--rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.0/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.0/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.0/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.0/README.md
--rw-r--r--   0        0        0    58121 2023-07-20 09:34:12.354036 lamindb_setup-0.49.0/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.0/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.0/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.0/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.0/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.0/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.0/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.0/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.0/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.0/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.0/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.0/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.0/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.0/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.0/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.49.0/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.0/lamin-project.yaml
--rw-r--r--   0        0        0     2757 2023-07-20 09:34:05.410170 lamindb_setup-0.49.0/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.49.0/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.49.0/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.49.0/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.49.0/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.0/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.0/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.49.0/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6600 2023-07-20 09:33:22.825129 lamindb_setup-0.49.0/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1413 2023-07-03 19:06:33.505992 lamindb_setup-0.49.0/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.49.0/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.49.0/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.0/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.49.0/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.0/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.0/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.0/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.49.0/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.0/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.0/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.49.0/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.0/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.49.0/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.0/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0    11191 2023-07-20 09:33:22.825771 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     4153 2023-07-20 09:33:22.826619 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-07-18 04:17:11.571437 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.0/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.49.0/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4583 2023-07-17 14:58:45.055809 lamindb_setup-0.49.0/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.49.0/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.0/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.0/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.0/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    31175 2023-07-17 17:14:39.802147 lamindb_setup-0.49.0/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.0/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.0/lnschema-core/README.md
--rw-r--r--   0        0        0      508 2023-07-17 17:14:39.802828 lamindb_setup-0.49.0/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.0/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
--rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.0/lnschema-core/lnschema_core/mocks.py
--rw-r--r--   0        0        0    33218 2023-07-17 17:14:39.803249 lamindb_setup-0.49.0/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.0/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.0/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.0/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.0/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.0/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.0/noxfile.py
--rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.49.0/pyproject.toml
--rw-r--r--   0        0        0     1170 2023-07-20 09:33:22.827762 lamindb_setup-0.49.0/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.0/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.0/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.0/tests/test_bionty.py
--rw-r--r--   0        0        0     2974 2023-07-17 14:58:45.056044 lamindb_setup-0.49.0/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.49.0/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.0/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-03 19:06:33.506543 lamindb_setup-0.49.0/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.0/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.0/tests/test_signup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.49.0/PKG-INFO
+-rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.1/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.1/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.1/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.1/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.1/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.1/README.md
+-rw-r--r--   0        0        0    58296 2023-07-25 01:45:03.871260 lamindb_setup-0.49.1/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.1/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.1/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.1/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.1/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.1/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.1/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.1/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.1/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.1/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.1/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.1/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.1/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.1/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.1/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.49.1/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.1/lamin-project.yaml
+-rw-r--r--   0        0        0     2757 2023-07-25 01:44:47.580795 lamindb_setup-0.49.1/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-07-24 10:00:44.787940 lamindb_setup-0.49.1/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.49.1/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.49.1/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.49.1/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.1/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.1/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.49.1/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6602 2023-07-25 01:43:24.440143 lamindb_setup-0.49.1/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1413 2023-07-24 10:02:47.316262 lamindb_setup-0.49.1/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.49.1/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.49.1/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.1/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.49.1/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.1/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.1/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.1/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.49.1/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.1/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.1/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.49.1/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.1/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.49.1/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.1/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.1/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0    11185 2023-07-25 01:43:24.440811 lamindb_setup-0.49.1/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     4686 2023-07-25 01:43:24.441037 lamindb_setup-0.49.1/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.1/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.49.1/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.1/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.1/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-07-18 04:17:11.571437 lamindb_setup-0.49.1/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.1/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.1/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.49.1/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4583 2023-07-17 14:58:45.055809 lamindb_setup-0.49.1/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.49.1/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.1/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.1/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.1/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.1/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.1/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    33450 2023-07-25 01:43:38.325656 lamindb_setup-0.49.1/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.1/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.1/lnschema-core/README.md
+-rw-r--r--   0        0        0      447 2023-07-25 01:43:38.325792 lamindb_setup-0.49.1/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.1/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
+-rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
+-rw-r--r--   0        0        0     3840 2023-07-25 01:43:38.325894 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0009_remove_featureset_files_feature_unit_and_more.py
+-rw-r--r--   0        0        0     2514 2023-07-25 01:43:38.325950 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0010_dataset_categories_file_categories.py
+-rw-r--r--   0        0        0     4324 2023-07-25 01:43:38.326033 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0011_label_remove_tag_created_by_remove_tag_parents_and_more.py
+-rw-r--r--   0        0        0     3585 2023-07-25 01:43:38.326104 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0012_remove_label_ref_id_remove_label_ref_orm_and_more.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.1/lnschema-core/lnschema_core/mocks.py
+-rw-r--r--   0        0        0    64949 2023-07-25 01:43:38.326395 lamindb_setup-0.49.1/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.1/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.1/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.1/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.1/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.1/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.1/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.49.1/pyproject.toml
+-rw-r--r--   0        0        0     2481 2023-07-25 01:43:24.441355 lamindb_setup-0.49.1/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.1/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.1/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.1/tests/test_bionty.py
+-rw-r--r--   0        0        0     4049 2023-07-25 01:43:24.441540 lamindb_setup-0.49.1/tests/test_init_instance.py
+-rw-r--r--   0        0        0     2207 2023-07-25 01:43:24.442039 lamindb_setup-0.49.1/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.1/tests/test_login.py
+-rw-r--r--   0        0        0      457 2023-07-24 10:02:47.316450 lamindb_setup-0.49.1/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.1/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.1/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.49.1/PKG-INFO
```

### Comparing `lamindb_setup-0.49.0/.github/workflows/build.yml` & `lamindb_setup-0.49.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.1/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/.gitignore` & `lamindb_setup-0.49.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/.pre-commit-config.yaml` & `lamindb_setup-0.49.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/LICENSE` & `lamindb_setup-0.49.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/changelog.md` & `lamindb_setup-0.49.1/docs/changelog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🐛 Fix flawed DBUser logic in `init_instance` | [442](https://github.com/laminlabs/lamindb-setup/pull/442) | [bpenteado](https://github.com/bpenteado) | 2023-07-24 | 0.49.1
 🗃️ Enable multiple DB access roles in instances (decompose connection string) | [431](https://github.com/laminlabs/lamindb-setup/pull/431) | [bpenteado](https://github.com/bpenteado) | 2023-07-19 | 0.49.0
 💚 Fix instability | [441](https://github.com/laminlabs/lamindb-setup/pull/441) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
 👷 Run CI against the staging environment | [440](https://github.com/laminlabs/lamindb-setup/pull/440) | [bpenteado](https://github.com/bpenteado) | 2023-07-18 |
 ♻️ Simplify `StorageSettings` | [439](https://github.com/laminlabs/lamindb-setup/pull/439) | [falexwolf](https://github.com/falexwolf) | 2023-07-17 | 0.48.8
 🔒️ Increase locker expiration time to 1 week | [437](https://github.com/laminlabs/lamindb-setup/pull/437) | [Koncopd](https://github.com/Koncopd) | 2023-07-08 | 0.48.7
 🚸 Import order of schema modules shouldn't matter | [436](https://github.com/laminlabs/lamindb-setup/pull/436) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.6
 🚸 Deal with legacy instances | [435](https://github.com/laminlabs/lamindb-setup/pull/435) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.5
```

### Comparing `lamindb_setup-0.49.0/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.49.1/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/faq/multi-session.ipynb` & `lamindb_setup-0.49.1/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.49.1/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.49.1/docs/faq/test-sqlite-sync.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.49.1/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.49.1/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.49.1/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.49.1/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/docs/guide/setup-user.md` & `lamindb_setup-0.49.1/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/__init__.py` & `lamindb_setup-0.49.1/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.49.0"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.49.1"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.49.0/lamindb_setup/__main__.py` & `lamindb_setup-0.49.1/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.49.1/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_close.py` & `lamindb_setup-0.49.1/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_delete.py` & `lamindb_setup-0.49.1/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_docstrings.py` & `lamindb_setup-0.49.1/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_init_instance.py` & `lamindb_setup-0.49.1/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_load_instance.py` & `lamindb_setup-0.49.1/lamindb_setup/_load_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     from ._check_instance_setup import check_instance_setup
 
     owner, name = get_owner_name_from_identifier(identifier)
 
     if check_instance_setup() and not _test:
         raise RuntimeError(
             "Currently don't support init or load of multiple instances in the same"
-            " Python sessionWe will bring this feature back at some point"
+            " Python session. We will bring this feature back at some point"
         )
     else:
         # compare normalized identifier with a potentially previously loaded identifier
         if (
             settings._instance_exists
             and f"{owner}/{name}" != settings.instance.identifier
         ):
```

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_migrate.py` & `lamindb_setup-0.49.1/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_notebook.py` & `lamindb_setup-0.49.1/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_register_instance.py` & `lamindb_setup-0.49.1/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_schema.py` & `lamindb_setup-0.49.1/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_set.py` & `lamindb_setup-0.49.1/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_settings.py` & `lamindb_setup-0.49.1/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_setup_user.py` & `lamindb_setup-0.49.1/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.49.1/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_django.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_hub_client.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_hub_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,17 +125,18 @@
             return "instance-exists-already"
 
         validate_unique_sqlite(
             hub=hub, db=db, storage_id=storage_id, name=name, account=account
         )
 
         instance_id = uuid4().hex
-        db_user_id = uuid4().hex
+        db_user_id = None
 
         if db_dsn:
+            db_user_id = uuid4().hex
             instance = sb_insert_instance(  # noqa
                 {
                     "id": instance_id,
                     "account_id": account["id"],
                     "name": name,
                     "storage_id": storage_id,
                     "db": db,
@@ -170,23 +171,23 @@
                     "schema_str": schema_str,
                     "public": False if public is None else public,
                     "description": description,
                 },
                 hub,
             )
 
-            sb_insert_collaborator(
-                {
-                    "instance_id": instance_id,
-                    "account_id": account["user_id"],
-                    "db_user_id": db_user_id,
-                    "role": "admin",
-                },
-                hub,
-            )
+        sb_insert_collaborator(
+            {
+                "instance_id": instance_id,
+                "account_id": account["user_id"],
+                "db_user_id": db_user_id,
+                "role": "admin",
+            },
+            hub,
+        )
 
         # upon successful insert of a new row in the instance table
         # (and all associated tables), return None
         # clients test for this return value, hence, don't change it
         return None
     except APIError as api_error:
         uq_instance_db_error = (
```

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_hub_crud.py`

 * *Files 14% similar despite different names*

```diff
@@ -48,14 +48,39 @@
         .data
     )
     if len(data) == 0:
         return None
     return data[0]
 
 
+def sb_update_instance(
+    instance_id: str, instance_fields: dict, supabase_client: Client
+):
+    data = (
+        supabase_client.table("instance")
+        .update(instance_fields)
+        .eq("id", instance_id)
+        .execute()
+        .data
+    )
+    if len(data) == 0:
+        return None
+    return data[0]
+
+
+def sb_delete_instance(
+    id: str,
+    supabase_client: Client,
+):
+    data = supabase_client.table("instance").delete().eq("id", id).execute().data
+    if len(data) == 0:
+        return None
+    return data[0]
+
+
 # --------------- COLLABORATOR ----------------------
 def sb_insert_collaborator(account_instance_fields: dict, supabase_client: Client):
     try:
         (
             supabase_client.table("account_instance")
             .insert(account_instance_fields, returning="minimal")
             .execute()
```

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_hub_utils.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lamindb_setup/dev/upath.py` & `lamindb_setup-0.49.1/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.49.1/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.1/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/.gitignore` & `lamindb_setup-0.49.1/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.49.1/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.49.1/lnschema-core/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🚚 Remove reference ORM from Label and add it to Feature, add slot to FeatureSet link models | [238](https://github.com/laminlabs/lnschema-core/pull/238) | [falexwolf](https://github.com/falexwolf) | 2023-07-24 |
+📝 Updated view_parents signature | [237](https://github.com/laminlabs/lnschema-core/pull/237) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-23 | 0.40.1
+🚚 More comprehensive `Label` and `FeatureSet` fields | [236](https://github.com/laminlabs/lnschema-core/pull/236) | [falexwolf](https://github.com/falexwolf) | 2023-07-23 |
+🚚 Integrate `Category` and `Tag` into `Label` | [235](https://github.com/laminlabs/lnschema-core/pull/235) | [falexwolf](https://github.com/falexwolf) | 2023-07-22 |
+🚚 Add `description` and `parents` to `Tag`, delete `Project`, replace `Run.name` with `Run.reference_type`, `Run.inputs` as `File.input_of` | [233](https://github.com/laminlabs/lnschema-core/pull/233) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
+🚚 Add categories to file and dataset | [232](https://github.com/laminlabs/lnschema-core/pull/232) | [falexwolf](https://github.com/falexwolf) | 2023-07-21 |
+💄 Improve docstring | [231](https://github.com/laminlabs/lnschema-core/pull/231) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-20 | 0.39.0
+🚚 Rename `FeatureValue` to `Category` | [230](https://github.com/laminlabs/lnschema-core/pull/230) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
+📝 Add examples to docstring | [229](https://github.com/laminlabs/lnschema-core/pull/229) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-19 |
+🚚 Move `feature_sets` to `File` instead of having `files` on `FeatureSet` | [228](https://github.com/laminlabs/lnschema-core/pull/228) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
+✨ Add `Feature.unit` | [227](https://github.com/laminlabs/lnschema-core/pull/227) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
+♻️ Refactor `Feature` and add `FeatureValue` | [225](https://github.com/laminlabs/lnschema-core/pull/225) | [falexwolf](https://github.com/falexwolf) | 2023-07-18 |
+🔥 Remove top_hit param from search | [226](https://github.com/laminlabs/lnschema-core/pull/226) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-18 |
 🍱 Added more methods for signature | [224](https://github.com/laminlabs/lnschema-core/pull/224) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-17 |
 🚚 Add `Transform.parents` and `File.hash_type` | [223](https://github.com/laminlabs/lnschema-core/pull/223) | [falexwolf](https://github.com/falexwolf) | 2023-07-07 | 0.38.3
 ✨ Add `from_df` and `from_anndata` to `File` | [222](https://github.com/laminlabs/lnschema-core/pull/222) | [falexwolf](https://github.com/falexwolf) | 2023-07-05 | 0.38.2
 💄 Do not show None fields | [221](https://github.com/laminlabs/lnschema-core/pull/221) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.38.1
 🚚 Move `QuerySet` to lamindb | [220](https://github.com/laminlabs/lnschema-core/pull/220) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 |
 ✨ Allow for annotate in `.df()` | [219](https://github.com/laminlabs/lnschema-core/pull/219) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 |
 🚚 Rename `File.name` to `File.description` | [218](https://github.com/laminlabs/lnschema-core/pull/218) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 | 0.38.0
```

### Comparing `lamindb_setup-0.49.0/lnschema-core/LICENSE` & `lamindb_setup-0.49.1/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.49.1/lnschema-core/lnschema_core/types.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/lnschema-core/pyproject.toml` & `lamindb_setup-0.49.1/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/noxfile.py` & `lamindb_setup-0.49.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/pyproject.toml` & `lamindb_setup-0.49.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/tests/hub/test_storage.py` & `lamindb_setup-0.49.1/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.49.0/tests/test_init_instance.py` & `lamindb_setup-0.49.1/tests/test_load_instance.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,86 +1,57 @@
-from pathlib import Path
-
 import lamindb_setup as ln_setup
 
-pgurl = "postgresql://postgres:pwd@0.0.0.0:5432/pgtest"
-
-
-def test_init_instance_postgres_default_name():
-    ln_setup.init(storage="./mydatapg", db=pgurl, _test=True)
-    assert ln_setup.settings.instance.name == "pgtest"
-    assert not ln_setup.settings.instance.storage.is_cloud
-    assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
-    assert ln_setup.settings.instance.dialect == "postgresql"
-    assert ln_setup.settings.instance.db == pgurl
-    assert (
-        ln_setup.settings.instance.storage.root.as_posix()
-        == Path("mydatapg").absolute().as_posix()
-    )
-    ln_setup.delete("pgtest")
+# from lamindb_setup.dev._hub_client import connect_hub_with_auth
+# from lamindb_setup.dev._hub_crud import (
+#     sb_delete_instance,
+#     sb_select_account_by_handle,
+#     sb_select_instance_by_name,
+#     sb_update_instance,
+# )
+from lamindb_setup.dev._settings_store import instance_settings_file
 
 
-def test_init_instance_postgres_custom_name():
-    ln_setup.init(storage="./mystorage", name="mydata2", db=pgurl, _test=True)
-    assert ln_setup.settings.instance.name == "mydata2"
-    assert not ln_setup.settings.instance.storage.is_cloud
-    assert ln_setup.settings.instance.owner == ln_setup.settings.user.handle
-    assert ln_setup.settings.instance.dialect == "postgresql"
-    assert ln_setup.settings.instance.db == pgurl
-    assert (
-        ln_setup.settings.instance.storage.root.as_posix()
-        == Path("mystorage").absolute().as_posix()
-    )
-    ln_setup.delete("mydata2")
-
-
-def test_init_instance_postgres_cloud_aws_us():
+def test_load_remote_instance():
+    ln_setup.login("testuser1")
+    ln_setup.delete("lndb-setup-ci")
     ln_setup.init(storage="s3://lndb-setup-ci", _test=True)
-    assert ln_setup.settings.storage.is_cloud
-    assert str(ln_setup.settings.storage.root) == "s3://lndb-setup-ci/"
-    assert ln_setup.settings.storage.root_as_str == "s3://lndb-setup-ci"
-    assert ln_setup.settings.storage.region == "us-east-1"
+    instance_settings_file("lndb-setup-ci", "testuser1").unlink()
+    ln_setup.load("testuser1/lndb-setup-ci", _test=True)
+    assert ln_setup.settings.instance.storage.is_cloud
+    assert ln_setup.settings.instance.storage.root_as_str == "s3://lndb-setup-ci"
     assert (
-        str(ln_setup.settings.instance._sqlite_file)
+        ln_setup.settings.instance._sqlite_file.as_posix()
         == "s3://lndb-setup-ci/lndb-setup-ci.lndb"
     )
+    # ln_setup.delete("lndb-setup-ci")
 
 
-def test_init_instance_postgres_cloud_aws_europe():
-    # do the same for an S3 bucket in Europe
-    ln_setup.init(
-        storage="s3://lndb-setup-ci-eu-central-1",
-        name="lndb-setup-ci-europe",
-        _test=True,
-    )
-    assert ln_setup.settings.storage.region == "eu-central-1"
-    assert ln_setup.settings.instance.name == "lndb-setup-ci-europe"
-    assert (
-        str(ln_setup.settings.instance._sqlite_file)
-        == "s3://lndb-setup-ci-eu-central-1/lndb-setup-ci-europe.lndb"
-    )
-
-
-# def test_db_unique_error():
+# def test_load_public_connection_string():
+#     # Admin connection strings are currently assigned to non-collaborator
+#     # users of public instances
+#     pgurl = "postgresql://postgres:pwd@0.0.0.0:5432/pgtest"
+#     ln_setup.login("testuser1")
+#     ln_setup.init(storage="./mydatapg", db=pgurl, _test=True)
+#     ln_setup.register()
+#     # Get hub instance entries and make it public
+#     hub = connect_hub_with_auth(access_token=ln_setup.settings.user.access_token)
+#     account = sb_select_account_by_handle(
+#         handle=ln_setup.settings.instance.owner, supabase_client=hub
+#     )
+#     instance = sb_select_instance_by_name(
+#         account_id=account["id"],
+#         name=ln_setup.settings.instance.name,
+#         supabase_client=hub,
+#     )
+#     sb_update_instance(
+#         instance_id=instance["id"],
+#         instance_fields={"public": True},
+#         supabase_client=hub,
+#     )
+#     # Load instance with non-collaborator user
 #     ln_setup.login("testuser2")
-
-#     # postgres
-
-
-# #     with pytest.raises(RuntimeError):
-# #         ln_setup.init(
-# #             storage="s3://lndb-setup-ci",
-# #             schema="retro, bionty",
-# #             db="postgresql://batman:robin@35.222.187.204:5432/retro",
-# #         )
-
-# # sqlite
-# # this fails because there is already an sqlite with the same name in that bucket
-# # hence, the sqlite file would clash
-
-# # with pytest.raises(RuntimeError):
-# #     ln_setup.init(storage="s3://lamindb-ci")
-
-
-# def test_value_error_schema():
-#     with pytest.raises(ModuleNotFoundError):
-#         ln_setup.init(storage="tmpstorage1", schema="bionty, xyz1")
+#     instance_settings_file("pgtest", "testuser1").unlink()
+#     ln_setup.load("testuser1/pgtest", _test=True)
+#     assert ln_setup.settings.instance.db == pgurl
+#     ln_setup.login("testuser1")
+#     ln_setup.delete("pgtest")
+#     sb_delete_instance(instance["id"], hub)
```

### Comparing `lamindb_setup-0.49.0/PKG-INFO` & `lamindb_setup-0.49.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.49.0
+Version: 0.49.1
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
```

