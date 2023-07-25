# Comparing `tmp/skip-django-is-core-2.24.7.2.tar.gz` & `tmp/skip-django-is-core-2.24.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-is-core-2.24.7.2.tar", last modified: Mon Mar 20 13:48:52 2023, max compression
+gzip compressed data, was "skip-django-is-core-2.24.7.3.tar", last modified: Tue Jul 25 14:05:56 2023, max compression
```

## Comparing `skip-django-is-core-2.24.7.2.tar` & `skip-django-is-core-2.24.7.3.tar`

### file list

```diff
@@ -1,263 +1,263 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/README
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/dynamo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/dynamo/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/dynamo/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/elasticsearch/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/elasticsearch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/forms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/field_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/http_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/rest_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/ui_ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/ui_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/dj/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/is_core/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/auth/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/auth/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/context_processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.890071 skip-django-is-core-2.24.7.2/is_core/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/cores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/0002_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.882071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/is_core/background_serialization.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/background_export/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/cores.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/cores.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/exceptions/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.894071 skip-django-is-core-2.24.7.2/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/boundfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/fieldset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/formsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/forms/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/add_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/detail_views.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/form_views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/generic_inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_form_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_objects_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_table_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/objects_views.py
--rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/generic_views/table_views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/loading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.882071 skip-django-is-core-2.24.7.2/is_core/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.882071 skip-django-is-core-2.24.7.2/is_core/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/models/humanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/models/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/patterns.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/rest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/paginators.py
--rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/rest/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.882071 skip-django-is-core-2.24.7.2/is_core/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/is_core/static/is_core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.898071 skip-django-is-core-2.24.7.2/is_core/static/is_core/css/
--rw-r--r--   0 runner    (1001) docker     (123)   277370 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/css/app.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.902071 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   136822 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   747545 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)   136516 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    92136 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78460 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    34350 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)   144714 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)    34052 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   204814 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)   917575 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)   204528 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   104280 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    80300 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.woff2
--rwxr-xr-x   0 runner    (1001) docker     (123)    32357 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.eot
--rwxr-xr-x   0 runner    (1001) docker     (123)    95652 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.svg
--rwxr-xr-x   0 runner    (1001) docker     (123)    56512 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.ttf
--rwxr-xr-x   0 runner    (1001) docker     (123)    35804 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.906071 skip-django-is-core-2.24.7.2/is_core/static/is_core/images/
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/images/arrow.png
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/images/cal.png
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/images/select-arrow.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.906071 skip-django-is-core-2.24.7.2/is_core/static/is_core/js/
--rw-r--r--   0 runner    (1001) docker     (123)  1054526 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/static/is_core/js/app.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.886071 skip-django-is-core-2.24.7.2/is_core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.906071 skip-django-is-core-2.24.7.2/is_core/templates/is_core/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/500.html
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/error.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.906071 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_field.html
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/inline_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/login_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/model_add_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/model_default_form.html
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/model_detail_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/responsive_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/responsive_inline_objects.html
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/stacked_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/tabular_inline_formset.html
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/tabular_inline_objects.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/add_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/base_table.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/default_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/detail_form.html
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/objects.html
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/readonly_detail.html
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/readonly_fieldset.html
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/rest_documentation.html
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/table.html
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/home.html
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/logged_out.html
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/login.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/bread_crumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/sub_menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/tabs_menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/templates/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templates/is_core/views/bulk-change-view.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templatetags/forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templatetags/menu.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templatetags/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/templatetags/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/crawler.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/data_generator_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/tests/factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/factory/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/rest_generic_test_cases.py
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/tests/ui_generic_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/utils/field_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/utils/models.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/is_core/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/views/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/views/csrf.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/is_core/views/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-20 13:48:43.000000 skip-django-is-core-2.24.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 13:48:52.910071 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-20 13:48:52.000000 skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.461264 skip-django-is-core-2.24.7.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 14:05:56.461264 skip-django-is-core-2.24.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/README
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.413264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/dynamo/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/dynamo/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.417264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/elasticsearch/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/elasticsearch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.417264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/forms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.417264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.421264 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/field_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/http_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7456 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/rest_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/ui_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/ui_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.421264 skip-django-is-core-2.24.7.3/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/dj/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      385 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.421264 skip-django-is-core-2.24.7.3/is_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/auth/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/auth/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/context_processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/cores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/commands/deleteexpiredexports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/0002_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3776 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.405264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/is_core/background_serialization.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.425264 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/background_export/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.429264 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.429264 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/cores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.429264 skip-django-is-core-2.24.7.3/is_core/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4484 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/exceptions/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.433264 skip-django-is-core-2.24.7.3/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/boundfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/fieldset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/formsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13940 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15024 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/forms/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.433264 skip-django-is-core-2.24.7.3/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/add_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9639 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/detail_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25720 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/form_views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.437264 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/generic_inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10444 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_form_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_table_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/objects_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14413 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/generic_views/table_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/loading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.409264 skip-django-is-core-2.24.7.3/is_core/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.409264 skip-django-is-core-2.24.7.3/is_core/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.437264 skip-django-is-core-2.24.7.3/is_core/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)    25101 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.437264 skip-django-is-core-2.24.7.3/is_core/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/models/humanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/models/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7687 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/patterns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.437264 skip-django-is-core-2.24.7.3/is_core/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/paginators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16501 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/rest/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.409264 skip-django-is-core-2.24.7.3/is_core/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.409264 skip-django-is-core-2.24.7.3/is_core/static/is_core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.437264 skip-django-is-core-2.24.7.3/is_core/static/is_core/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   277370 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/css/app.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.445264 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)   136822 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   747545 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   136516 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    92136 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78460 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    34350 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   144714 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    34052 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13548 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   204814 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   917575 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   204528 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   104280 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    80300 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.woff2
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32357 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.eot
+-rwxr-xr-x   0 runner    (1001) docker     (123)    95652 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.svg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56512 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.ttf
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35804 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.445264 skip-django-is-core-2.24.7.3/is_core/static/is_core/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/images/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/images/cal.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/images/select-arrow.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.445264 skip-django-is-core-2.24.7.3/is_core/static/is_core/js/
+-rw-r--r--   0 runner    (1001) docker     (123)  1054526 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/static/is_core/js/app.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.409264 skip-django-is-core-2.24.7.3/is_core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.449264 skip-django-is-core-2.24.7.3/is_core/templates/is_core/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/error.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.453264 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_field.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/inline_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/login_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/model_add_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/model_default_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/model_detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/responsive_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/responsive_inline_objects.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/stacked_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/tabular_inline_formset.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/tabular_inline_objects.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.453264 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/add_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8763 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/base_table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/default_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/detail_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/objects.html
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/readonly_detail.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/readonly_fieldset.html
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/rest_documentation.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/table.html
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/logged_out.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/login.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.453264 skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/bread_crumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/sub_menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/tabs_menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.457264 skip-django-is-core-2.24.7.3/is_core/templates/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templates/is_core/views/bulk-change-view.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.457264 skip-django-is-core-2.24.7.3/is_core/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templatetags/forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templatetags/menu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templatetags/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/templatetags/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.457264 skip-django-is-core-2.24.7.3/is_core/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/crawler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/data_generator_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.457264 skip-django-is-core-2.24.7.3/is_core/tests/factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/factory/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/rest_generic_test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/tests/ui_generic_test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.457264 skip-django-is-core-2.24.7.3/is_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14518 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/utils/field_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/utils/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.461264 skip-django-is-core-2.24.7.3/is_core/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/views/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/views/csrf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/is_core/views/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:05:56.461264 skip-django-is-core-2.24.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-07-25 14:05:47.000000 skip-django-is-core-2.24.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:05:56.461264 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8376 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-25 14:05:56.000000 skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/top_level.txt
```

### Comparing `skip-django-is-core-2.24.7.2/LICENSE` & `skip-django-is-core-2.24.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/PKG-INFO` & `skip-django-is-core-2.24.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.24.7.2
+Version: 2.24.7.3
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-is-core-2.24.7.2/README.md` & `skip-django-is-core-2.24.7.3/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/__init__.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/cores/resources.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/cores/resources.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/dynamo/core.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/dynamo/core.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/elasticsearch/models.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/forms/__init__.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0001_initial.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0002_auto_20210401_1128.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/migrations/0003_issue_parent.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/models.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/dynamo.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/elasticsearch.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/factories.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/field_permissions.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/field_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/http_exceptions.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/permissions.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/rest.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/rest.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/rest_permissions.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/rest_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/test_case.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/ui_ordering.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/ui_ordering.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/ui_permissions.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/ui_permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/apps/issue_tracker/tests/utils.py` & `skip-django-is-core-2.24.7.3/example/dj/apps/issue_tracker/tests/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/settings/base.py` & `skip-django-is-core-2.24.7.3/example/dj/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/settings/settings.py` & `skip-django-is-core-2.24.7.3/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/example/dj/wsgi.py` & `skip-django-is-core-2.24.7.3/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/actions.py` & `skip-django-is-core-2.24.7.3/is_core/actions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/auth/permissions.py` & `skip-django-is-core-2.24.7.3/is_core/auth/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/auth/views.py` & `skip-django-is-core-2.24.7.3/is_core/auth/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/config.py` & `skip-django-is-core-2.24.7.3/is_core/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/cores.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/management/commands/deleteexpiredexports.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/management/commands/deleteexpiredexports.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/0001_initial.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/migrations/0002_migration.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/migrations/0002_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/models.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/resource.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/tasks.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/tasks.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/templates/is_core/generic_views/table.html` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/templates/is_core/generic_views/table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/background_export/views.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/background_export/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/cores.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/dynamo/views.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/dynamo/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/cores.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/cores.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/filters.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/contrib/elasticsearch/views.py` & `skip-django-is-core-2.24.7.3/is_core/contrib/elasticsearch/views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/exceptions/response.py` & `skip-django-is-core-2.24.7.3/is_core/exceptions/response.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/boundfield.py` & `skip-django-is-core-2.24.7.3/is_core/forms/boundfield.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/fields.py` & `skip-django-is-core-2.24.7.3/is_core/forms/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/fieldset.py` & `skip-django-is-core-2.24.7.3/is_core/forms/fieldset.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/forms.py` & `skip-django-is-core-2.24.7.3/is_core/forms/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/formsets.py` & `skip-django-is-core-2.24.7.3/is_core/forms/formsets.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/generic.py` & `skip-django-is-core-2.24.7.3/is_core/forms/generic.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/models.py` & `skip-django-is-core-2.24.7.3/is_core/forms/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/patch.py` & `skip-django-is-core-2.24.7.3/is_core/forms/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/utils.py` & `skip-django-is-core-2.24.7.3/is_core/forms/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/forms/widgets.py` & `skip-django-is-core-2.24.7.3/is_core/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/add_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/add_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/base.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/detail_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/detail_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/form_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/form_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/base.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/generic_inline_form_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/generic_inline_form_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_form_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_form_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_objects_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_objects_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/inline_table_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/inline_table_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/inlines/permissions.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/inlines/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/mixins.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/mixins.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/objects_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/objects_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/generic_views/table_views.py` & `skip-django-is-core-2.24.7.3/is_core/generic_views/table_views.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/loading.py` & `skip-django-is-core-2.24.7.3/is_core/loading.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/locale/cs/LC_MESSAGES/django.mo` & `skip-django-is-core-2.24.7.3/is_core/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/locale/cs/LC_MESSAGES/django.po` & `skip-django-is-core-2.24.7.3/is_core/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/main.py` & `skip-django-is-core-2.24.7.3/is_core/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -228,15 +228,16 @@
     def get_default_ordering(self):
         return self.default_ordering if self.default_ordering is not None else (self.model._meta.ordering or ('pk',))
 
     def preload_queryset(self, request, qs):
         return qs
 
     def get_queryset(self, request):
-        return self.model._default_manager.get_queryset().order_by(*self.get_default_ordering())
+        # Add PK to make ordering deterministic
+        return self.model._default_manager.get_queryset().order_by(*self.get_default_ordering(), 'pk')
 
 
 class UiCore(Core):
     """Main core for UI views."""
 
     abstract = True
```

### Comparing `skip-django-is-core-2.24.7.2/is_core/menu.py` & `skip-django-is-core-2.24.7.3/is_core/menu.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/middleware.py` & `skip-django-is-core-2.24.7.3/is_core/middleware.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/models/patch.py` & `skip-django-is-core-2.24.7.3/is_core/models/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/patterns.py` & `skip-django-is-core-2.24.7.3/is_core/patterns.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/rest/datastructures.py` & `skip-django-is-core-2.24.7.3/is_core/rest/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/rest/filters.py` & `skip-django-is-core-2.24.7.3/is_core/rest/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/rest/paginators.py` & `skip-django-is-core-2.24.7.3/is_core/rest/paginators.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/rest/resource.py` & `skip-django-is-core-2.24.7.3/is_core/rest/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/site.py` & `skip-django-is-core-2.24.7.3/is_core/site.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/css/app.css` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/css/app.css`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.eot` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.svg` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.ttf` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.woff` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-brands-400.woff2` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.eot` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.svg` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.ttf` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.woff` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-regular-400.woff2` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.eot` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.svg` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.ttf` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.woff` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/fa-solid-900.woff2` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.eot` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.eot`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.svg` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.svg`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.ttf` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.ttf`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/fonts/icon-works-webfont.woff` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/fonts/icon-works-webfont.woff`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/images/arrow.png` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/images/arrow.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/images/cal.png` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/images/cal.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/images/select-arrow.png` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/images/select-arrow.png`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/static/is_core/js/app.js` & `skip-django-is-core-2.24.7.3/is_core/static/is_core/js/app.js`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/base.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/base.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_field.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_field.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_fieldset.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/default_form.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/inline_table.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/inline_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/model_default_form.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/model_default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/responsive_inline_formset.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/responsive_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/responsive_inline_objects.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/responsive_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/stacked_inline_formset.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/stacked_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/tabular_inline_formset.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/tabular_inline_formset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/forms/tabular_inline_objects.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/forms/tabular_inline_objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/base_table.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/base_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/default_form.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/default_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/detail_form.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/detail_form.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/objects.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/objects.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/generic_views/readonly_fieldset.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/generic_views/readonly_fieldset.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/logged_out.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/logged_out.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/login.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/login.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templates/is_core/menu/menu.html` & `skip-django-is-core-2.24.7.3/is_core/templates/is_core/menu/menu.html`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templatetags/forms.py` & `skip-django-is-core-2.24.7.3/is_core/templatetags/forms.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templatetags/menu.py` & `skip-django-is-core-2.24.7.3/is_core/templatetags/menu.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templatetags/permissions.py` & `skip-django-is-core-2.24.7.3/is_core/templatetags/permissions.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/templatetags/utils.py` & `skip-django-is-core-2.24.7.3/is_core/templatetags/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/tests/crawler.py` & `skip-django-is-core-2.24.7.3/is_core/tests/crawler.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/tests/data_generator_test_case.py` & `skip-django-is-core-2.24.7.3/is_core/tests/data_generator_test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/tests/factory/fields.py` & `skip-django-is-core-2.24.7.3/is_core/tests/factory/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/tests/rest_generic_test_cases.py` & `skip-django-is-core-2.24.7.3/is_core/tests/rest_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/tests/ui_generic_test_cases.py` & `skip-django-is-core-2.24.7.3/is_core/tests/ui_generic_test_cases.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/utils/__init__.py` & `skip-django-is-core-2.24.7.3/is_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/utils/decorators.py` & `skip-django-is-core-2.24.7.3/is_core/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/utils/field_api.py` & `skip-django-is-core-2.24.7.3/is_core/utils/field_api.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/is_core/utils/models.py` & `skip-django-is-core-2.24.7.3/is_core/utils/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/setup.py` & `skip-django-is-core-2.24.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/PKG-INFO` & `skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-is-core
-Version: 2.24.7.2
+Version: 2.24.7.3
 Summary: Information systems core.
 Home-page: https://github.com/skip-pay/django-is-core
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Keywords: django,admin,information systems,REST
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `skip-django-is-core-2.24.7.2/skip_django_is_core.egg-info/SOURCES.txt` & `skip-django-is-core-2.24.7.3/skip_django_is_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

