# Comparing `tmp/oarepo-model-builder-files-4.0.3.tar.gz` & `tmp/oarepo-model-builder-files-4.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-4.0.3.tar", last modified: Tue Jun 27 09:01:25 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-4.0.4.tar", last modified: Tue Jul 25 20:51:30 2023, max compression
```

## Comparing `oarepo-model-builder-files-4.0.3.tar` & `oarepo-model-builder-files-4.0.4.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/parent_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/files_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/pid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/service.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/parent_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 09:01:25.164016 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-27 09:01:25.000000 oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-27 09:01:25.168016 oarepo-model-builder-files-4.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 08:57:21.000000 oarepo-model-builder-files-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.381062 oarepo-model-builder-files-4.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-25 20:51:30.381062 oarepo-model-builder-files-4.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.357062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.361062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.365062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.365062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.369062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.369062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/parent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.373062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.373062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (123)    12123 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.373062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.373062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.377062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.381062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/files_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.381062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 20:51:30.361062 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 20:51:30.000000 oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-07-25 20:51:30.381062 oarepo-model-builder-files-4.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 20:46:23.000000 oarepo-model-builder-files-4.0.4/setup.py
```

### Comparing `oarepo-model-builder-files-4.0.3/PKG-INFO` & `oarepo-model-builder-files-4.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.3
+Version: 4.0.4
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.3/README.md` & `oarepo-model-builder-files-4.0.4/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/__init__.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/builtin_models/invenio_files.json` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/builtin_models/invenio_files.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/__init__.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/file.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/file.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,17 @@
     affects = [DefaultsModelComponent]
 
     class ModelSchema(ma.Schema):
         files = ma.fields.Nested(get_file_schema)
 
     def process_links(self, datatype, section: Section, **kwargs):
         if self.is_record_profile:
+            has_files = 'files' in datatype.definition
+            if not has_files:
+                return
             # add files link item
             has_files = False
             for link in section.config["links_item"]:
                 if link.name == "files":
                     has_files = True
             if not has_files:
                 section.config["links_item"].append(
```

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/__init__.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/defaults.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/files_field.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/files_field.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/permissions.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/pid.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/record.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/resource.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/files_model/service.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/files_model/service.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/datatypes/components/parent_record.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/datatypes/components/parent_record.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,14 +17,17 @@
         RecordMetadataModelComponent,
         ServiceModelComponent,
     ]
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         if context["profile"] != "record":
             return
+        # have files plugin in virtualenv but there are no files in the record
+        if 'files' not in datatype.definition:
+            return
         prepend_array(datatype, "record-metadata", "base-classes", "RecordMetadataBase")
         prepend_array(datatype, "record-metadata", "base-classes", "db.Model")
 
         append_array(
             datatype,
             "record-metadata",
             "imports",
```

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files/profiles/file.py` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files/profiles/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         **kwargs,
     ):
         # get parent record. In most cases, it has already been prepared and is reused
         # from cache. It files profile is called the first, then this will call prepare({})
         # on the record and will take some time (no files will be generated, only class names
         # allocated)
         parent_record = model.get_schema_section("record", model_path[:-1])
+        if 'files' not in parent_record.definition:
+            return
 
         file_profile = dict_get(model.schema, model_path)
         file_profile.setdefault("type", "file")
 
         # pass the parent record as an extra context item. This will be handled by file-aware
         # components in their "prepare" method
         super().build(
```

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.3
+Version: 4.0.4
 Description-Content-Type: text/markdown
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
 Files are represented as another ("file") record connected with the original parent one.
 The plugin generates the file record and modifies the parent record to create connection with new file one.
```

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/oarepo_model_builder_files.egg-info/entry_points.txt` & `oarepo-model-builder-files-4.0.4/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.3/setup.cfg` & `oarepo-model-builder-files-4.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-files
-version = 4.0.3
+version = 4.0.4
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

