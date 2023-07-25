# Comparing `tmp/skip-django-pyston-2.16.5.1.tar.gz` & `tmp/skip-django-pyston-2.16.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pyston-2.16.5.1.tar", last modified: Tue Jan 31 14:04:56 2023, max compression
+gzip compressed data, was "skip-django-pyston-2.16.5.2.tar", last modified: Tue Jul 25 14:10:02 2023, max compression
```

## Comparing `skip-django-pyston-2.16.5.1.tar` & `skip-django-pyston-2.16.5.2.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.948372 skip-django-pyston-2.16.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-31 14:04:56.948372 skip-django-pyston-2.16.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.920372 skip-django-pyston-2.16.5.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.920372 skip-django-pyston-2.16.5.1/example/dj/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.920372 skip-django-pyston-2.16.5.1/example/dj/apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.920372 skip-django-pyston-2.16.5.1/example/dj/apps/app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.924372 skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.924372 skip-django-pyston-2.16.5.1/example/dj/apps/app/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/elasticsearch/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.924372 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0002_user_manual_created_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0004_issue_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.928372 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/cors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/elasticsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/extra_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    29627 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/fieldsets.py
--rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/standard_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.928372 skip-django-pyston-2.16.5.1/example/dj/settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/dj/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/example/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.932372 skip-django-pyston-2.16.5.1/pyston/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.932372 skip-django-pyston-2.16.5.1/pyston/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.936372 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.936372 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/order.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.936372 skip-django-pyston-2.16.5.1/pyston/converters/
--rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/converters/extra.py
--rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/converters/file_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/data_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.940372 skip-django-pyston-2.16.5.1/pyston/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/django_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/filters/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.940372 skip-django-pyston-2.16.5.1/pyston/forms/
--rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/forms/postgres.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.916372 skip-django-pyston-2.16.5.1/pyston/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.916372 skip-django-pyston-2.16.5.1/pyston/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.940372 skip-django-pyston-2.16.5.1/pyston/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/metamodel.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.944372 skip-django-pyston-2.16.5.1/pyston/order/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/django_sorters.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/sorters.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/order/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.944372 skip-django-pyston-2.16.5.1/pyston/requested_fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/requested_fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/requested_fields/managers.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/requested_fields/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    41564 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/response.py
--rw-r--r--   0 runner    (1001) docker     (123)    35172 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.944372 skip-django-pyston-2.16.5.1/pyston/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/templates/default_pdf_table.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.944372 skip-django-pyston-2.16.5.1/pyston/templates/pyston/
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/templates/pyston/html_converter.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.944372 skip-django-pyston-2.16.5.1/pyston/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/datastructures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/pyston/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 14:04:56.948372 skip-django-pyston-2.16.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-31 14:04:48.000000 skip-django-pyston-2.16.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 14:04:56.948372 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-31 14:04:56.000000 skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/dj/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/dj/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/dj/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/example/dj/apps/app/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/elasticsearch/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.174843 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0002_user_manual_created_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0003_auto_20170729_2305.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0004_issue_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4865 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.174843 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8155 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/cors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5080 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/elasticsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/extra_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29627 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/fieldsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17672 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15447 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/standard_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.174843 skip-django-pyston-2.16.5.2/example/dj/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/dj/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/example/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)    15487 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/converters/extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5446 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/converters/file_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/data_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.178843 skip-django-pyston-2.16.5.2/pyston/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/django_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9178 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16715 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/filters/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/forms/
+-rw-r--r--   0 runner    (1001) docker     (123)    35083 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/forms/postgres.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/pyston/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.170843 skip-django-pyston-2.16.5.2/pyston/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     6725 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/metamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/order/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/django_sorters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11029 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/sorters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/order/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/requested_fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/requested_fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/requested_fields/managers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/requested_fields/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41564 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35172 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/templates/default_pdf_table.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/templates/pyston/
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/templates/pyston/html_converter.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/pyston/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     9811 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/pyston/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-25 14:09:49.000000 skip-django-pyston-2.16.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 14:10:02.182844 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-25 14:10:02.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-25 14:10:02.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:10:02.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 14:10:01.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-25 14:10:02.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-25 14:10:02.000000 skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/top_level.txt
```

### Comparing `skip-django-pyston-2.16.5.1/AUTHORS.txt` & `skip-django-pyston-2.16.5.2/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/LICENSE` & `skip-django-pyston-2.16.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/PKG-INFO` & `skip-django-pyston-2.16.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.1
+Version: 2.16.5.2
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pyston-2.16.5.1/README.md` & `skip-django-pyston-2.16.5.2/README.md`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/models.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/dynamo/resource.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/elasticsearch/models.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/elasticsearch/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0001_initial.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/migrations/0003_auto_20170729_2305.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/migrations/0003_auto_20170729_2305.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/models.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/models.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/resource.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/serializable.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/serializable.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/compatibility.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/cors.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/cors.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/dynamo.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/dynamo.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/elasticsearch.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/extra_resource.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/extra_resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/factories.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/factories.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/fields.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/fields.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/fieldsets.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/fieldsets.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/filter.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/order.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/serializer.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/serializer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/standard_operations.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/standard_operations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/apps/app/tests/test_case.py` & `skip-django-pyston-2.16.5.2/example/dj/apps/app/tests/test_case.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/settings/base.py` & `skip-django-pyston-2.16.5.2/example/dj/settings/base.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/settings/settings.py` & `skip-django-pyston-2.16.5.2/example/dj/settings/settings.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/urls.py` & `skip-django-pyston-2.16.5.2/example/dj/urls.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/example/dj/wsgi.py` & `skip-django-pyston-2.16.5.2/example/dj/wsgi.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/cache.py` & `skip-django-pyston-2.16.5.2/pyston/cache.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/conf.py` & `skip-django-pyston-2.16.5.2/pyston/conf.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/filter.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/filter.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/order.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/paginator.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/paginator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/dynamo/resource.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/dynamo/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/filters.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/order.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/order.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/contrib/elasticsearch/resource.py` & `skip-django-pyston-2.16.5.2/pyston/contrib/elasticsearch/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/converters/__init__.py` & `skip-django-pyston-2.16.5.2/pyston/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/converters/extra.py` & `skip-django-pyston-2.16.5.2/pyston/converters/extra.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/converters/file_generators.py` & `skip-django-pyston-2.16.5.2/pyston/converters/file_generators.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/data_processor.py` & `skip-django-pyston-2.16.5.2/pyston/data_processor.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/exception.py` & `skip-django-pyston-2.16.5.2/pyston/exception.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/filters/django_filters.py` & `skip-django-pyston-2.16.5.2/pyston/filters/django_filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/filters/filters.py` & `skip-django-pyston-2.16.5.2/pyston/filters/filters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/filters/managers.py` & `skip-django-pyston-2.16.5.2/pyston/filters/managers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/filters/parser.py` & `skip-django-pyston-2.16.5.2/pyston/filters/parser.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/filters/utils.py` & `skip-django-pyston-2.16.5.2/pyston/filters/utils.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/forms/__init__.py` & `skip-django-pyston-2.16.5.2/pyston/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/forms/postgres.py` & `skip-django-pyston-2.16.5.2/pyston/forms/postgres.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/locale/cs/LC_MESSAGES/django.mo` & `skip-django-pyston-2.16.5.2/pyston/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/locale/cs/LC_MESSAGES/django.po` & `skip-django-pyston-2.16.5.2/pyston/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/metamodel.py` & `skip-django-pyston-2.16.5.2/pyston/metamodel.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/order/django_sorters.py` & `skip-django-pyston-2.16.5.2/pyston/order/django_sorters.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/order/managers.py` & `skip-django-pyston-2.16.5.2/pyston/order/managers.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,8 +215,8 @@
 
 class DjangoOrderManager(BaseParserModelOrderManager, BaseDjangoOrderManager):
     """
     Manager that uses parser to parse input order data to the list of order strings.
     """
 
     def _sort_queryset(self, qs, terms):
-        return qs.order_by(*terms)
+        return qs.order_by(*terms, 'pk')  # Add PK to make ordering deterministic
```

### Comparing `skip-django-pyston-2.16.5.1/pyston/order/parsers.py` & `skip-django-pyston-2.16.5.2/pyston/order/parsers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/paginator.py` & `skip-django-pyston-2.16.5.2/pyston/paginator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/patch.py` & `skip-django-pyston-2.16.5.2/pyston/patch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/requested_fields/managers.py` & `skip-django-pyston-2.16.5.2/pyston/requested_fields/managers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/requested_fields/parser.py` & `skip-django-pyston-2.16.5.2/pyston/requested_fields/parser.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/resource.py` & `skip-django-pyston-2.16.5.2/pyston/resource.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/response.py` & `skip-django-pyston-2.16.5.2/pyston/response.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/serializer.py` & `skip-django-pyston-2.16.5.2/pyston/serializer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/templates/default_pdf_table.html` & `skip-django-pyston-2.16.5.2/pyston/templates/default_pdf_table.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/templates/pyston/html_converter.html` & `skip-django-pyston-2.16.5.2/pyston/templates/pyston/html_converter.html`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/__init__.py` & `skip-django-pyston-2.16.5.2/pyston/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/compatibility.py` & `skip-django-pyston-2.16.5.2/pyston/utils/compatibility.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/datastructures.py` & `skip-django-pyston-2.16.5.2/pyston/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/decorators.py` & `skip-django-pyston-2.16.5.2/pyston/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/files.py` & `skip-django-pyston-2.16.5.2/pyston/utils/files.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/pyston/utils/helpers.py` & `skip-django-pyston-2.16.5.2/pyston/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/setup.py` & `skip-django-pyston-2.16.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/PKG-INFO` & `skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pyston
-Version: 2.16.5.1
+Version: 2.16.5.2
 Summary: Pyston is a Django mini-framework creating APIs.
 Home-page: https://github.com/skip-pay/django-pyston
 Author: Lubos Matl
 Author-email: matllubos@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pyston-2.16.5.1/skip_django_pyston.egg-info/SOURCES.txt` & `skip-django-pyston-2.16.5.2/skip_django_pyston.egg-info/SOURCES.txt`

 * *Files identical despite different names*

