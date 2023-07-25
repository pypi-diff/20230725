# Comparing `tmp/invenio-records-lom-0.8.1.tar.gz` & `tmp/invenio-records-lom-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-records-lom-0.8.1.tar", last modified: Fri Apr 28 11:55:34 2023, max compression
+gzip compressed data, was "invenio-records-lom-0.9.0.tar", last modified: Thu Jun  1 10:49:51 2023, max compression
```

## Comparing `invenio-records-lom-0.8.1.tar` & `invenio-records-lom-0.9.0.tar`

### file list

```diff
@@ -1,162 +1,176 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/babel.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.430551 invenio-records-lom-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.430551 invenio-records-lom-0.8.1/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/fixtures/demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/lomrecords/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/relations.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15953 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/services/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/pids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     6483 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/records.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/services.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/services/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/results.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/record.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/export.html
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/files.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/
--rw-r--r--   0 runner    (1001) docker     (123)     4945 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/uploads.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/translations/messages.pot
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.438551 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     6242 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/deposits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/records/records.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
--rw-r--r--   0 runner    (1001) docker     (123)     7442 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
--rw-r--r--   0 runner    (1001) docker     (123)    10784 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
--rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
--rw-r--r--   0 runner    (1001) docker     (123)    11560 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.426551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/invenio_records_lom/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/learning_resource_types.json
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/utils/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/invenio_records_lom/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.434551 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5028 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 11:55:34.000000 invenio-records-lom-0.8.1/invenio_records_lom.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/requirements-devel.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3851 2023-04-28 11:55:34.446551 invenio-records-lom-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:55:34.442551 invenio-records-lom-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2539 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_invenio_records_lom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_pids_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-28 11:55:27.000000 invenio-records-lom-0.8.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.186571 invenio-records-lom-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-01 10:49:51.186571 invenio-records-lom-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/babel.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/fixtures/demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/lomrecords/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/lomrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/jsonschemas/lomrecords/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.166570 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/datacite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8057 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/schemas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/pids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/records.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/services.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/services/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.166570 invenio-records-lom-0.9.0/invenio_records_lom/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/static/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.178570 invenio-records-lom-0.9.0/invenio_records_lom/static/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/static/templates/invenio_records_lom/results.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/record.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/export.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/files.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/uploads.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/translations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9685 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/translations/messages.pot
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7848 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/deposits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/records/records.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11506 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13135 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.170570 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.182571 invenio-records-lom-0.9.0/invenio_records_lom/upgrade_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/upgrade_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/upgrade_scripts/migrate_0_8_to_0_9.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.186571 invenio-records-lom-0.9.0/invenio_records_lom/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    64221 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    64211 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/utils/learning_resource_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/utils/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/invenio_records_lom/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.174570 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-01 10:49:51.000000 invenio-records-lom-0.9.0/invenio_records_lom.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/requirements-devel.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      737 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-01 10:49:51.186571 invenio-records-lom-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:49:51.186571 invenio-records-lom-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/test_invenio_records_lom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/test_pids_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/test_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-01 10:49:45.000000 invenio-records-lom-0.9.0/tests/test_utils.py
```

### Comparing `invenio-records-lom-0.8.1/.editorconfig` & `invenio-records-lom-0.9.0/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/CHANGES.rst` & `invenio-records-lom-0.9.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,24 @@
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-06-01)
+
+- add `format` and `resource-type` to upload-page
+- add schema for cleaner OAI-PMH-output
+- add "$schema"-key to jsons in database
+- update landing page
+- implement and configure permissions
+- fix image-preview by implementing iiif-resource
+
+
 Version v0.8.1 (release 2023-04-28)
 
 - upload: require license permission
 
 
 Version v0.8.0 (release 2023-04-20)
```

### Comparing `invenio-records-lom-0.8.1/CONTRIBUTING.rst` & `invenio-records-lom-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/INSTALL.rst` & `invenio-records-lom-0.9.0/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/LICENSE` & `invenio-records-lom-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/MANIFEST.in` & `invenio-records-lom-0.9.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/PKG-INFO` & `invenio-records-lom-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.8.1
+Version: 0.9.0
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -45,28 +45,39 @@
         
 .. image:: https://readthedocs.org/projects/invenio-records-lom/badge/?version=latest
         :target: https://invenio-records-lom.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
 
-invenio data model for Learning object metadata
+Invenio module that adds a data model based on LOM (Learning Object Metadata).
+The specification of the LOM-dialect used by this module can be found here: `LOM-UIBK (only available in german) <https://oer-repo.uibk.ac.at/lom/latest/>`_
 
 Further documentation is available on
 https://invenio-records-lom.readthedocs.io/
 
 ..
     Copyright (C) 2020 Graz University of Technology.
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-06-01)
+
+- add `format` and `resource-type` to upload-page
+- add schema for cleaner OAI-PMH-output
+- add "$schema"-key to jsons in database
+- update landing page
+- implement and configure permissions
+- fix image-preview by implementing iiif-resource
+
+
 Version v0.8.1 (release 2023-04-28)
 
 - upload: require license permission
 
 
 Version v0.8.0 (release 2023-04-20)
```

### Comparing `invenio-records-lom-0.8.1/README.rst` & `invenio-records-lom-0.9.0/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -22,11 +22,12 @@
         
 .. image:: https://readthedocs.org/projects/invenio-records-lom/badge/?version=latest
         :target: https://invenio-records-lom.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
 
-invenio data model for Learning object metadata
+Invenio module that adds a data model based on LOM (Learning Object Metadata).
+The specification of the LOM-dialect used by this module can be found here: `LOM-UIBK (only available in german) <https://oer-repo.uibk.ac.at/lom/latest/>`_
 
 Further documentation is available on
 https://invenio-records-lom.readthedocs.io/
```

### Comparing `invenio-records-lom-0.8.1/babel.ini` & `invenio-records-lom-0.9.0/babel.ini`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/docs/Makefile` & `invenio-records-lom-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/docs/conf.py` & `invenio-records-lom-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/docs/index.rst` & `invenio-records-lom-0.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/docs/make.bat` & `invenio-records-lom-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/config.py` & `invenio-records-lom-0.9.0/invenio_records_lom/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,27 @@
 """Default configuration."""
 
 import idutils
 from flask_babelex import gettext as _
 from invenio_rdm_records.services.pids import providers
 
 from .resources.serializers import LOMToDataCite44Serializer
+from .services.permissions import LOMRecordPermissionPolicy
 from .services.pids import LOMDataCitePIDProvider
 
 LOM_BASE_TEMPLATE = "invenio_records_lom/base.html"
 
+#
+# Permission Configuration
+#
+LOM_PERMISSION_POLICY = LOMRecordPermissionPolicy
+
+#
+# Search Configuration
+#
 LOM_FACETS = {}
 
 LOM_SORT_OPTIONS = {
     "bestmatch": {
         "title": _("Best match"),
         "fields": ["_score"],  # ES defaults to desc on `_score` field
     },
@@ -30,14 +39,17 @@
 }
 
 LOM_SEARCH = {
     "sort": ["bestmatch", "newest"],
 }
 """Record search configuration."""
 
+#
+# HTML-Request Configuration
+#
 LOM_ROUTES = {
     # the blueprint prefixes `/lom` to these routes
     "uploads": "/uploads",
     "deposit_create": "/uploads/new",
     "deposit_edit": "/uploads/<pid_value>",
     "record_detail": "/<pid_value>",
     "record_export": "/<pid_value>/export/<export_format>",
@@ -53,14 +65,17 @@
         "name": _("JSON"),
         "serializer": "flask_resources.serializers:JSONSerializer",
         "content-type": "application/json",
         "filename": "{id}.json",
     },
 }
 
+#
+# Schema Configuration
+#
 LOM_RESOURCE_TYPES = [
     "course",
     "unit",
     "file",
     "link",
     "upload",
 ]
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ext.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ext.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 #
 # Copyright (C) 2020 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Flask extension for invenio-records-lom."""
+from invenio_rdm_records.resources import IIIFResource
+from invenio_rdm_records.services import IIIFService
 from invenio_rdm_records.services.pids import PIDManager, PIDsService
 from invenio_records_resources.resources import FileResource
 from invenio_records_resources.services import FileService
 
 from . import config
 from .resources import (
     LOMDraftFilesResourceConfig,
+    LOMIIIFResourceConfig,
     LOMRecordFilesResourceConfig,
     LOMRecordResource,
     LOMRecordResourceConfig,
 )
 from .services import (
     LOMDraftFilesServiceConfig,
     LOMRecordFilesServiceConfig,
@@ -68,23 +71,34 @@
         self.records_service = LOMRecordService(
             config=record_service_config,
             files_service=FileService(files_service_config),
             draft_files_service=FileService(draft_files_config),
             pids_service=PIDsService(record_service_config, PIDManager),
         )
 
+        # pylint: disable-next=attribute-defined-outside-init
+        self.iiif_service = IIIFService(
+            records_service=self.records_service, config=None
+        )
+
     def init_resources(self, app):  # pylint: disable=unused-argument
         """Initialize resouces."""
         # pylint: disable-next=attribute-defined-outside-init
         self.draft_files_resource = FileResource(
             config=LOMDraftFilesResourceConfig,
             service=self.records_service.draft_files,
         )
 
         # pylint: disable-next=attribute-defined-outside-init
+        self.iiif_resource = IIIFResource(
+            config=LOMIIIFResourceConfig,
+            service=self.iiif_service,
+        )
+
+        # pylint: disable-next=attribute-defined-outside-init
         self.record_files_resource = FileResource(
             config=LOMRecordFilesResourceConfig,
             service=self.records_service.files,
         )
 
         # pylint: disable-next=attribute-defined-outside-init
         self.records_resource = LOMRecordResource(
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/fixtures/demo.py` & `invenio-records-lom-0.9.0/invenio_records_lom/fixtures/demo.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/oai.py` & `invenio-records-lom-0.9.0/invenio_records_lom/oai.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/api.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,20 @@
 # relations =  # validate then clean assigned relations
 # schema =  # add second validation via jsonschema
 
 from invenio_drafts_resources.records import Draft, Record
 from invenio_drafts_resources.records.api import ParentRecord
 from invenio_pidstore.models import PIDStatus
 from invenio_rdm_records.records.systemfields import DraftStatus
-from invenio_records.systemfields import DictField, ModelField, RelationsField
+from invenio_records.systemfields import (
+    ConstantField,
+    DictField,
+    ModelField,
+    RelationsField,
+)
 from invenio_records_resources.records.api import FileRecord
 from invenio_records_resources.records.systemfields import (
     FilesField,
     IndexField,
     PIDField,
     PIDStatusCheckField,
 )
@@ -133,14 +138,15 @@
     access = RecordAccessField()
     bucket_id = ModelField(dump=False)
     bucket = ModelField(dump=False)
     index = IndexField("lomrecords-drafts-draft-v1.0.0", search_alias="lomrecords")
     is_published = PIDStatusCheckField(status=PIDStatus.REGISTERED, dump=True)
     pids = DictField()
     resource_type = DictField()
+    schema = ConstantField("$schema", "local://lomrecords/records/record-v1.0.0.json")
     status = DraftStatus()
 
 
 LOMFileDraft.record_cls = LOMDraft
 
 
 class LOMFileRecord(FileRecord):
@@ -178,11 +184,12 @@
     bucket = ModelField(dump=False)
     index = IndexField(
         "lomrecords-records-record-v1.0.0", search_alias="lomrecords-records"
     )
     is_published = PIDStatusCheckField(status=PIDStatus.REGISTERED, dump=True)
     pids = DictField()
     resource_type = DictField()
+    schema = ConstantField("$schema", "local://lomrecords/records/record-v1.0.0.json")
     status = DraftStatus()
 
 
 LOMFileRecord.record_cls = LOMRecord
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json` & `invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json` & `invenio-records-lom-0.9.0/invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/models.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/models.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/context.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/context.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/providers.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/providers.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/relations.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/relations.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/resolver.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/resolver.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/records/systemfields/results.py` & `invenio-records-lom-0.9.0/invenio_records_lom/records/systemfields/results.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/resources/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2021 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
-"""Invenio-Records-LOM module for creating REST APIs."""
+"""High-level API for working with LOM records, files, pids and search."""
 
 from .config import (
-    LOMDraftFilesResourceConfig,
-    LOMRecordFilesResourceConfig,
-    LOMRecordResourceConfig,
+    LOMDraftFilesServiceConfig,
+    LOMRecordFilesServiceConfig,
+    LOMRecordServiceConfig,
 )
-from .resources import LOMRecordResource
+from .permissions import LOMRecordPermissionPolicy
+from .services import LOMRecordService
 
 __all__ = (
-    "LOMDraftFilesResourceConfig",
-    "LOMRecordFilesResourceConfig",
-    "LOMRecordResource",
-    "LOMRecordResourceConfig",
+    "LOMDraftFilesServiceConfig",
+    "LOMRecordPermissionPolicy",
+    "LOMRecordFilesServiceConfig",
+    "LOMRecordService",
+    "LOMRecordServiceConfig",
 )
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/resources/config.py` & `invenio-records-lom-0.9.0/invenio_records_lom/resources/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """REST API configuration."""
 
 import marshmallow
 from flask_resources import JSONSerializer, ResponseHandler
+from invenio_rdm_records.resources import IIIFResourceConfig
 from invenio_records_resources.resources import RecordResourceConfig
 from invenio_records_resources.resources.files import FileResourceConfig
 
 from .serializers import LOMUIJSONSerializer
 
 record_serializer = {
     "application/json": ResponseHandler(JSONSerializer()),
@@ -53,7 +54,14 @@
 
     request_view_args = {
         "pid_value": marshmallow.fields.Str(),
         "scheme": marshmallow.fields.Str(),
     }
 
     response_handlers = record_serializer
+
+
+class LOMIIIFResourceConfig(IIIFResourceConfig):
+    """LOM IIIF Resource Config."""
+
+    blueprint_name = "lom_iiif"
+    url_prefix = "/lom/iiif"
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/resources/resources.py` & `invenio-records-lom-0.9.0/invenio_records_lom/resources/resources.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/resources/serializers/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/resources/serializers/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 #
 # Copyright (C) 2021 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Serializers turning records into html-template-insertable dicts."""
+from collections.abc import Mapping
 from copy import deepcopy
 
 from flask_resources import BaseListSchema, MarshmallowSerializer
 from flask_resources.serializers import JSONSerializer, MarshmallowJSONSerializer
 from lxml.builder import ElementMaker  # pylint: disable=no-name-in-module
 
-from .schemas import LOMToDataCite44Schema, LOMUIRecordSchema
+from .schemas import LOMMetadataToOAISchema, LOMToDataCite44Schema, LOMUIRecordSchema
 
 
 class LOMUIJSONSerializer(MarshmallowSerializer):
     """Wrapper with some convenience functions around a marshmallow-schema."""
 
     def __init__(self):
         """Initialize serializer with arguments for LOM-serialization."""
@@ -48,15 +49,28 @@
             "https://w3id.org/oerbase/profiles/lomuibk/latest/ "
             "https://w3id.org/oerbase/profiles/lomuibk/latest/lom-uibk.xsd"
         )
     }
 
     def __init__(self, metadata, lom_id, oaiserver_id_prefix, doi):
         """Constructor."""
-        self.metadata = metadata
+        # metadata might be out of order, and includes extraneous fields
+        # sort and filter with marshmallow:
+        # TODO: clean some of this up in database rather than here
+        metadata = deepcopy(metadata)
+        if "lifeCycle" in metadata:
+            # convert old capitalization to new one (note the capitalization of the 'C')
+            metadata["lifecycle"] = metadata.pop("lifeCycle")
+        if "metaMetadata" in metadata:
+            # convert old capitalization to new one (note the capitalization of the second 'M')
+            metadata["metametadata"] = metadata.pop("metaMetadata")
+        try:
+            self.metadata = LOMMetadataToOAISchema().load(metadata)
+        except Exception:  # pylint: disable=broad-exception-caught
+            self.metadata = metadata
         self.lom_id = lom_id
         self.oaiserver_id_prefix = oaiserver_id_prefix
         self.doi = doi
         self.element_maker = ElementMaker(namespace=self.NSMAP["lom"], nsmap=self.NSMAP)
 
     @property
     def repository_identifier(self):
@@ -87,36 +101,39 @@
         }
 
         return [jsn]
 
     def build_langstring(self, jsn, parent_tag):
         """Append XML corresponding to `jsn` to `parent_tag`.
 
-        `jsn` has to be of form `{"lang": "lang-name", "#text": "any_text"}`.
+        `jsn` has to either be of form `{"lang": "lang-name", "#text": "any_text"}`,
+        or be of form {"#text": "any_text"}.
         """
         if "lang" in jsn:
             tag = self.element_maker.langstring(
                 jsn["#text"],
                 **{"{http://www.w3.org/XML/1998/namespace}lang": jsn["lang"]},
             )
         else:
             tag = self.element_maker.langstring(jsn["#text"])
         parent_tag.append(tag)
 
     def build_location(self, jsn, parent_tag):
         """Append location to parent_tag."""
         tag = self.element_maker.location(
             jsn["#text"],
-            **{"{http://www.w3.org/XML/1998/namespace}lang": jsn["type"]},
+            # while some of LOM-UIBK's examples include a type-attribute here, most don't
+            # the `lom-uibk.xsd` also forbids extra attributes in this place...
         )
         parent_tag.append(tag)
 
     def build(self, jsn, parent_tag, inner_tag=None):
         """Walk through `jsn`, append its corresponding XML to `parent_tag`."""
-        if isinstance(jsn, dict):
+        # `LOMMetadataToOAISchema` returns a mix of `dict`s and `OrderedDict`s, check against common parent-class `Mapping`
+        if isinstance(jsn, Mapping):
             for key, value in jsn.items():
                 if key == "identifier":
                     for lst in [
                         self.repository_identifier,
                         self.repository_doi_identifier,
                     ]:
                         self.build(lst, parent_tag, self.element_maker("identifier"))
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/components.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/components.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/config.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,23 +14,27 @@
 )
 from invenio_drafts_resources.services.records.config import (
     RecordServiceConfig,
     is_draft,
     is_record,
 )
 from invenio_rdm_records.services.components import AccessComponent, MetadataComponent
-from invenio_rdm_records.services.config import has_doi, is_record_and_has_doi
+from invenio_rdm_records.services.config import (
+    has_doi,
+    is_iiif_compatible,
+    is_record_and_has_doi,
+)
 from invenio_records_resources.services import (
     ConditionalLink,
     FileLink,
     FileServiceConfig,
     Link,
     RecordLink,
 )
-from invenio_records_resources.services.base.config import ConfiguratorMixin
+from invenio_records_resources.services.base.config import ConfiguratorMixin, FromConfig
 
 from ..records import LOMDraft, LOMRecord
 from .components import LOMPIDsComponent, ResourceTypeComponent
 from .permissions import LOMRecordPermissionPolicy
 from .schemas import LOMRecordSchema
 
 
@@ -85,16 +89,17 @@
     # Record and draft class
     draft_cls = LOMDraft
     record_cls = LOMRecord
 
     # Schemas
     schema = LOMRecordSchema
 
-    permission_policy_cls = LOMRecordPermissionPolicy
-
+    permission_policy_cls = FromConfig(
+        "LOM_PERMISSION_POLICY", default=LOMRecordPermissionPolicy, import_string=True
+    )
     # PIDConfiguration
     pids_providers = FromConfigLOMPIDsProviders()
     pids_required = FromConfigLOMRequiredPIDs()
 
     # links
     links_item = {
         "doi": Link(
@@ -150,31 +155,42 @@
 
 
 class LOMDraftFilesServiceConfig(FileServiceConfig, ConfiguratorMixin):
     """Config for LOM draft files service."""
 
     record_cls = LOMDraft
     permission_action_prefix = "draft_"
-    permission_policy_cls = LOMRecordPermissionPolicy
+    permission_policy_cls = FromConfig(
+        "LOM_PERMISSION_POLICY", default=LOMRecordPermissionPolicy, import_string=True
+    )
 
     # links to appear within FileList-result:
     file_links_list = {
         "self": RecordLink("{+api}/lom/{id}/draft/files"),
     }
 
     # links to appear within the items of FileList-results:
     # (note that, due to `Link.should_render`, some of these links may not appear on items)
     file_links_item = {
         "commit": FileLink("{+api}/lom/{id}/draft/files/{key}/commit"),
         "content": FileLink("{+api}/lom/{id}/draft/files/{key}/content"),
+        "iiif_base": FileLink(
+            "{+api}/lom/iiif/draft:{id}:{key}", when=is_iiif_compatible
+        ),
         "self": FileLink("{+api}/lom/{id}/draft/files/{key}"),
     }
 
 
 class LOMRecordFilesServiceConfig(FileServiceConfig, ConfiguratorMixin):
     """Config for LOM files service."""
 
     record_cls = LOMRecord
-    permission_policy_cls = LOMRecordPermissionPolicy
+    permission_policy_cls = FromConfig(
+        "LOM_PERMISSION_POLICY", default=LOMRecordPermissionPolicy, import_string=True
+    )
 
     file_links_list = {}
-    file_links_item = {}
+    file_links_item = {
+        "iiif_base": FileLink(
+            "{+api}/lom/iiif/record:{id}:{key}", when=is_iiif_compatible
+        ),
+    }
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/permissions.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/permissions/policy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,51 +1,54 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright (C) 2021 Graz University of Technology.
+# Copyright (C) 2021-2023 Graz University of Technology.
 #
 # invenio-records-lom is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
-"""Permission-config classes for LOMRecordService-objects."""
+"""Permission-policy class for LOMRecordService-objects."""
 
 from invenio_rdm_records.services.generators import (
     IfFileIsLocal,
     IfRestricted,
     RecordOwners,
-    SecretLinks,
 )
 from invenio_rdm_records.services.permissions import RDMRecordPermissionPolicy
 from invenio_records_permissions.generators import (
     AnyUser,
     AuthenticatedUser,
     SystemProcess,
 )
 
+from .generators import OERCertifiedUsers, OERCurators
+
 
 class LOMRecordPermissionPolicy(RDMRecordPermissionPolicy):
     """Flask-principal style permissions for LOM record services.
 
     Note that the invenio_access.Permission parent-class always adds
     ``superuser-access``, so admin-Identities are always allowed to take any action.
     """
 
     # no rights for CommunityCurators, as this package doesn't implement communities
     # no rights for SubmissionReviewers, as this package doesn't implement reviews
     #
-    # General permission-categories, to be used in below categories
+    # General permission-groups, to be used in below categories
     #
     can_manage = [RecordOwners(), SystemProcess()]
-    can_curate = can_manage + [SecretLinks("edit")]
+    can_curate = can_manage + [OERCurators()]
     can_review = can_curate
-    can_preview = can_manage + [SecretLinks("preview")]
-    can_view = can_manage + [SecretLinks("view")]
+    can_preview = can_manage
+    can_view = can_manage
 
     can_authenticated = [AuthenticatedUser(), SystemProcess()]
     can_all = [AnyUser(), SystemProcess()]
 
+    can_handle_oer = [OERCertifiedUsers(), OERCurators(), SystemProcess()]
+
     #
     #  Records
     #
     # Allow searching of records
     can_search = can_all
     # Allow reading metadata of a record
     can_read = [
@@ -57,21 +60,21 @@
     ]
     can_get_content_files = [
         # note: even though this is closer to business logic than permissions,
         # it was simpler and less coupling to implement this as permission check
         IfFileIsLocal(then_=can_read_files, else_=[SystemProcess()]),
     ]
     # Allow submitting new record
-    can_create = can_authenticated
+    can_create = can_handle_oer
 
     #
     # Drafts
     #
     # Allow ability to search drafts
-    can_search_drafts = can_authenticated
+    can_search_drafts = can_handle_oer
     # Allow reading metadata of a draft
     can_read_draft = can_preview
     # Allow reading files of a draft
     can_draft_read_files = can_preview
     # Allow updating metadata of a draft
     can_update_draft = can_review
     # Allow uploading, updating and deleting files in drafts
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/pids.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/pids.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/fields.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/fields.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/metadata.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -97,35 +97,80 @@
     role = fields.Dict()
     entity = fields.List(
         fields.String(validate=validate.Length(min=1, error="Name cannot be empty."))
     )
 
 
 class LifecycleSchema(Schema):
-    """Schema for Lom's `lifecycle category."""
+    """Schema for LOM's `lifecycle` category."""
 
     contribute = fields.List(
         fields.Nested(ContributeSchema()),
         validate=validate.Length(min=1, error="Enter at least one contribution."),
     )
 
 
+class LocationSchema(Schema):
+    """Schema for LOM's `technical.location`."""
+
+    text = fields.String(attribute="#text", data_key="#text")
+
+
+class TechnicalSchema(Schema):
+    """Schema for LOM's `technical` category."""
+
+    format = fields.List(
+        fields.String(
+            required=True,
+            validate=validate.Length(min=1, error="Missing data for required field."),
+        ),
+        validate=validate.Length(min=1, max=1, error="Must enter exactly one format."),
+    )
+    location = fields.Nested(LocationSchema)
+
+
+class LearningResourceTypeSchema(Schema):
+    """Scheam for LOM's `educational.learningresourcetype`."""
+
+    source = fields.Field(
+        required=True,
+        validate=validate.Equal(
+            {
+                "langstring": {
+                    "#text": "https://w3id.org/kim/hcrt/scheme",
+                    "lang": "x-none",
+                }
+            }
+        ),
+    )
+    id = fields.String(
+        required=True,
+        validate=validate.Length(min=1, error="Missing data for required field."),
+    )
+
+
+class EducationalSchema(Schema):
+    """Schema for LOM's `educational` category."""
+
+    learningresourcetype = fields.Nested(LearningResourceTypeSchema, required=True)
+
+
 class RightsSchema(Schema):
     """Schema for LOM's `rights`-category."""
 
     copyrightandotherrestrictions = fields.Dict()
     description = fields.Dict()
     url = fields.String(
         required=True,
         validate=validate.Length(min=1, error="Missing data for required field."),
     )
 
 
 class TaxonSchema(Schema):
-    """Schema for Lom's `classification.taxonpath.taxon`-category."""
+    """Schema for LOM's `classification.taxonpath.taxon`-category."""
 
     id = fields.String(
         required=True,
         validate=validate.Regexp(
             r"https://w3id.org/oerbase/vocabs/oefos2012/\d+",
             error="Not a valid OEFOS-url.",
         ),
@@ -186,14 +231,16 @@
         unknown = INCLUDE
 
     # passed by parent as to multiplex, removed by parent affter load/dump
     type = fields.Field(validate=validate.Equal("upload"))
 
     general = fields.Nested(GeneralSchema, required=True)
     lifecycle = fields.Nested(LifecycleSchema, required=True)
+    technical = fields.Nested(TechnicalSchema, rquired=True)
+    educational = fields.Nested(EducationalSchema, required=True)
     rights = fields.Nested(RightsSchema, required=True)
     classification = fields.Nested(
         ClassificationSchema,
         many=True,
         required=True,
         validate=validate.Length(min=1, error="Must add OEFOS-classification."),
     )
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/schemas/records.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/schemas/records.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/services.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/services.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/services/tasks.py` & `invenio-records-lom-0.9.0/invenio_records_lom/services/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/static/templates/invenio_records_lom/results.html` & `invenio-records-lom-0.9.0/invenio_records_lom/static/templates/invenio_records_lom/results.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
       <p style="font-weight: bold">
         {{_('To use the upload feature, have your account activated by sending your OER certificate issued by the national
         certification body to <a href="mailto:telucation@tugraz.at">telucation@tugraz.at</a>.')}}
       </p>
 
       <p>
         {{_('Not yet certified? Members of Graz University of Technology are required to obtain the OER certificate from
-        fnma at Graz University of Technology, which you can obatin as part of the in-house training. Please register
+        fnma at Graz University of Technology, which you can obtain as part of the in-house training. Please register
         via your business card in <a href="online.tugraz.at">TUGRAZonline</a>.')}}
       </p>
 
       <p>
         {{_('As a member of another university, visit the information page on OER certification to find a corresponding
         offer at your university and submit your certificate to <a href="mailto:telucation@tugraz.at">telucation@tugraz.at</a>,
         after which an upload is possible.')}}
```

#### html2text {}

```diff
@@ -20,15 +20,15 @@
 transferred to OERhub.at - a national search engine for OER - in order to reach
 an even greater audience reach.')}}
 {{_('To use the upload feature, have your account activated by sending your OER
 certificate issued by the national certification body to
 telucation@tugraz.at.')}}
 {{_('Not yet certified? Members of Graz University of Technology are required
 to obtain the OER certificate from fnma at Graz University of Technology, which
-you can obatin as part of the in-house training. Please register via your
+you can obtain as part of the in-house training. Please register via your
 business card in TUGRAZonline.')}}
 {{_('As a member of another university, visit the information page on OER
 certification to find a corresponding offer at your university and submit your
 certificate to telucation@tugraz.at, after which an upload is possible.')}}
 {{_('For further information, please contact the OU Educational Technology
 directly at +43(316)873-8577 or write an email to telucation@tugraz.at.')}}
 {% endblock page_body %}
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/deposit.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/deposit.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/export.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/export.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/files.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/files.html`

 * *Files 14% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 #}
 {#
   NOTE:
   copy-pasted code from invenio_app_rdm/records/detail.html
   copy-pasting was necessary to use custom `box`es which override standard-endpoints with lom-endpoints
 #}
 
-{%- from "invenio_records_lom/records/macros/files.html" import lom_file_list_box, lom_preview_file_box %}
+{% from "invenio_records_lom/records/macros/files.html" import lom_file_list_box, lom_preview_file_box %}
 
-{%- if record.files.enabled -%}
-  {%- if permissions.can_read_files -%}
-    {# record has files AND user can see files #}
-    {%- set files = files|order_entries %}
-    {%- if files|has_previewable_files -%}
-      {%-set preview_file = files|select_preview_file(default_preview=record.files.default_preview) %}
-      {{ lom_preview_file_box(preview_file, pid, is_preview, record) }}
-    {%- endif -%}
-    {{ lom_file_list_box(files, pid, is_preview, record) }}
-  {% else %}
-    {# record has files BUT user cannot see files #}
-    <div class="panel-spacing">
-      <div class="ui accordion panel {{ record.ui.access_status.id }}" id="preview" href="#collapsablePreview">
-        <div class="active title panel-heading {{ record.ui.access_status.id }}">
-          {{ _("Files") }}
-          <i class="angle down icon"></i>
-        </div>
-        <div id="collapsablePreview" class="active content">
-          <div class="ui {{ record.ui.access_status.message_class }} message file-box-message">
-            <i class="ui {{ record.ui.access_status.icon }} icon"></i><b>{{ record.ui.access_status.title_l10n }}</b>
-            <p>{{ record.ui.access_status.description_l10n }}</p>
-            {% if record.access.embargo.reason %}
-              <p>{{_("Reason")}}: {{record.access.embargo.reason}}</p>
-            {% endif%}
+{% if record.files.enabled %}
+  <section id="record-files" class="rel-mt-2" aria-label="{{ _('Files') }}">
+    {% if permissions.can_read_files %}
+      {# record has files AND user can see files #}
+      <h2 id="files-heading">{{ _("Files") }}</h2>
+      {% set files = files|order_entries %}
+      {% if files|has_previewable_files %}
+        {% set preview_file = files|select_preview_file(default_preview=record.files.default_preview) %}
+        {{ lom_preview_file_box(preview_file, pid, is_preview, record) }}
+      {% endif %}
+      {{ lom_file_list_box(files, pid, is_preview, record) }}
+    {% else %}
+      {# record has files BUT user cannot see files #}
+      <div class="pt-0 pb-20">
+        <div class="ui accordion panel mb-10 {{ record.ui.access_status.id }}" id="preview" href="#collapsablePreview">
+          <div class="active title panel-heading {{ record.ui.access_status.id }}">
+            {{ _("Files") }}
+            <i class="angle down icon"></i>
+          </div>
+          <div id="collapsablePreview" class="active content rm-pt">
+            <div class="ui {{ record.ui.access_status.message_class }} message file-box-message">
+              <i class="ui {{ record.ui.access_status.icon }} icon"></i><b>{{ record.ui.access_status.title_l10n }}</b>
+              <p>{{ record.ui.access_status.description_l10n }}</p>
+              {% if record.access.embargo.reason %}
+                <p>{{_("Reason")}}: {{record.access.embargo.reason}}</p>
+              {% endif %}
+            </div>
           </div>
         </div>
       </div>
-    </div>
-  {%- endif %}
-{%- endif %}
+    {% endif %}
+  </section>
+{% endif %}
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/macros/files.html`

 * *Files 10% similar despite different names*

```diff
@@ -31,98 +31,113 @@
     src="{{ preview_url }}">
   </iframe>
 {%- endmacro %}
 
 
 {% macro lom_preview_file_box(file, pid, is_preview, record) %}
 <div class="">
-  <div class="ui accordion panel {{record.ui.access_status.id}}" id="preview" href="#collapsablePreview">
-    <div class="active title panel-heading {{record.ui.access_status.id}} truncated">
-      {{file.key}}
-      <i class="ui angle down icon"></i>
+  <div class="ui accordion panel mb-10 {{record.ui.access_status.id}}" id="preview" href="#collapsablePreview">
+    <div class="active title trigger panel-heading {{record.ui.access_status.id}} truncated" tabindex="0" aria-label="{{ _('File preview') }}">
+      <span id="preview-file-title">{{file.key}}</span>
+      <i class="ui angle right icon"></i>
     </div>
-    <div id="collapsablePreview" class="active content">
+    <div id="collapsablePreview" class="active content pt-0">
       <div>
         {{ preview_file('invenio_records_lom.record_file_preview', pid_value=pid, filename=file.key, is_preview=is_preview) }}
       </div>
     </div>
   </div>
 </div>
 {%- endmacro %}
 
 
-{%- macro file_list(files, pid, is_preview, with_preview=true, download_endpoint='invenio_records_lom.record_file_download', preview_endpoint='invenio_records_lom.record_file_preview') %}
+{%- macro file_list(
+  files,
+  pid,
+  is_preview,
+  with_preview=true,
+  download_endpoint='invenio_records_lom.record_file_download',
+  preview_endpoint='invenio_records_lom.record_file_preview'
+) %}
   <table class="ui striped table files-table">
     <thead>
       <tr>
         <th>{{_('Name')}}</th>
         <th>{{_('Size')}}</th>
+        {# TODO: invenio does archive-download here; if that were implemented for lom-records, we can use invenio's macro and remove this macro... #}
         <th></th>
       </tr>
     </thead>
     <tbody>
-    {% for file in files %}
-      {% if is_preview %}
-        {%- set file_url_download = url_for(download_endpoint, pid_value=pid, filename=file.key, download=1, preview=1) %}
-        {%- set file_url_preview = url_for(preview_endpoint, pid_value=pid, filename=file.key, preview=1) %}
-      {% else %}
-        {%- set file_url_download = url_for(download_endpoint, pid_value=pid, filename=file.key, download=1) %}
-        {%- set file_url_preview = url_for(preview_endpoint, pid_value=pid, filename=file.key) %}
-      {% endif %}
-      {%- set file_type = file.key.split('.')[-1] %}
-      <tr>
-        <td>
-          <div class="truncated">
-            <a href="{{ file_url_download }}">{{ file.key }}</a>
-          </div>
-          <small class="ui text-muted font-tiny">{{ file.checksum }}
-          <div class="ui icon inline-block" data-tooltip="{{_('This is the file fingerprint (checksum), which can be used to verify the file integrity.')}}">
-            <i class="question circle checksum icon"></i>
-          </div>
-          </small>
-        </td>
-        <td>{{ file.size|filesizeformat }}</td>
-        <td class="right aligned">
-          <span>
-            {% if with_preview and file_type|lower is previewable %}
-            <a class="ui compact mini button preview-link" href="{{ file_url_preview }}" target="preview-iframe" data-file-key="{{file.key}}">
-              <i class="eye icon"></i> {{_("Preview")}}
-            </a>
-            {% endif %}
-            <a class="ui compact mini button" href="{{ file_url_download }}">
-              <i class="download icon"></i>
-              {{_('Download')}}
-            </a>
-          </span>
-        </td>
-      </tr>
-    {% endfor %}
+      {% for file in files %}
+        {% if is_preview %}
+          {%- set file_url_download = url_for(download_endpoint, pid_value=pid, filename=file.key, download=1, preview=1) %}
+          {%- set file_url_preview = url_for(preview_endpoint, pid_value=pid, filename=file.key, preview=1) %}
+        {% else %}
+          {%- set file_url_download = url_for(download_endpoint, pid_value=pid, filename=file.key, download=1) %}
+          {%- set file_url_preview = url_for(preview_endpoint, pid_value=pid, filename=file.key) %}
+        {% endif %}
+        {%- set file_type = file.key.split('.')[-1] %}
+        <tr>
+          <td>
+            <div class="truncated">
+              <a href="{{ file_url_download }}">{{ file.key }}</a>
+            </div>
+            <small class="ui text-muted font-tiny">
+              {{ file.checksum }}
+              <div class="ui icon inline-block" data-tooltip="{{_('This is the file fingerprint (checksum), which can be used to verify the file integrity.')}}">
+                <i class="question circle checksum icon"></i>
+              </div>
+            </small>
+          </td>
+          <td>{{ file.size|filesizeformat(binary=not config.APP_RDM_DISPLAY_DECIMAL_FILE_SIZES) }}</td>
+          <td class="right aligned">
+            <span>
+              {% if with_preview and file_type|lower is previewable %}
+              <a class="ui compact mini button preview-link" href="{{ file_url_preview }}" target="preview-iframe" data-file-key="{{file.key}}">
+                <i class="eye icon"></i>
+                {{_("Preview")}}
+              </a>
+              {% endif %}
+              <a class="ui compact mini button" href="{{ file_url_download }}" role="button">
+                <i class="download icon"></i>
+                {{_('Download')}}
+              </a>
+            </span>
+          </td>
+        </tr>
+      {% endfor %}
     </tbody>
   </table>
 {%- endmacro %}
 
 
 {% macro lom_file_list_box(files, pid, is_preview, record) %}
-<div class="">
-  <div class="ui accordion panel {{record.ui.access_status.id}}" id="preview" href="#collapsablePreview">
-    <div class="active title panel-heading {{record.ui.access_status.id}}">
-      {{ _("Files") }}
-      <small class="text-muted">{% if files %} ({{files|sum(attribute='size')|filesizeformat}}){% endif %}</small>
-      <i class="angle down icon"></i>
-    </div>
-    <div class="active content">
-      {% if record.access.files == 'restricted' %}
-      <div class="ui {{ record.ui.access_status.message_class }} message file-box-message">
-        <i class="ui {{ record.ui.access_status.icon }} icon"></i><b>{{ record.ui.access_status.title_l10n }}</b>
-        <p>{{ record.ui.access_status.description_l10n }}</p>
-        {% if record.access.embargo.reason %}
-          <p>{{_("Reason")}}: {{record.access.embargo.reason}}</p>
-        {% endif%}
+  <div class="">
+    <div class="ui accordion panel mb-10 {{record.ui.access_status.id}}" id="preview" href="#collapsablePreview">
+      <div class="active title trigger panel-heading {{record.ui.access_status.id}}" tabindex="0">
+        {{ _("Files") }}
+        <small class="text-muted">
+          {% if files %}
+            ({{files|sum(attribute='size')|filesizeformat}})
+          {% endif %}
+        </small>
+        <i class="angle right icon"></i>
       </div>
-      {% endif %}
-      <div id="collapsableFiles">
-        {{ file_list(files, pid, is_preview) }}
+      <div class="active content pt-0">
+        {% if record.access.files == 'restricted' %}
+          <div class="ui {{ record.ui.access_status.message_class }} message file-box-message">
+            <i class="ui {{ record.ui.access_status.icon }} icon"></i>
+            <b>{{ record.ui.access_status.title_l10n }}</b>
+            <p>{{ record.ui.access_status.description_l10n }}</p>
+            {% if record.access.embargo.reason %}
+              <p>{{_("Reason")}}: {{record.access.embargo.reason}}</p>
+            {% endif%}
+          </div>
+        {% endif %}
+        <div id="collapsableFiles">
+          {{ file_list(files, pid, is_preview) }}
+        </div>
       </div>
     </div>
   </div>
-</div>
 {%- endmacro %}
```

#### html2text {}

```diff
@@ -11,30 +11,30 @@
 url_for(preview_endpoint, pid_value=pid_value, filename=filename, preview=1) -
 %} {% else %} {%- set preview_url = url_for(preview_endpoint,
 pid_value=pid_value, filename=filename) -%} {% endif %}   {%- endmacro %} {%
 macro lom_preview_file_box(file, pid, is_preview, record) %}
 {{file.key}}
 {{ preview_file('invenio_records_lom.record_file_preview', pid_value=pid,
 filename=file.key, is_preview=is_preview) }}
-{%- endmacro %} {%- macro file_list(files, pid, is_preview, with_preview=true,
+{%- endmacro %} {%- macro file_list( files, pid, is_preview, with_preview=true,
 download_endpoint='invenio_records_lom.record_file_download',
-preview_endpoint='invenio_records_lom.record_file_preview') %}
-{{_('Name')}}       {{_('Size')}}
-                                                 {% if with_preview and
-                                                file_type|lower is previewable
-{{_file.key_}}      {{ file.size|filesizeformat %}
-{{ file.checksum }} }}                           {{_("Preview")}}
-                                                 {% endif %}
-                                                 {{_('Download')}}
+preview_endpoint='invenio_records_lom.record_file_preview' ) %}
+{{_('Name')}}    {{_('Size')}}
+                                                             {% if with_preview
+                                                            and file_type|lower
+{{_file.key_}}   {{ file.size|filesizeformat(binary=not     is previewable %}
+{{ file.checksum config.APP_RDM_DISPLAY_DECIMAL_FILE_SIZES)  {{_("Preview")}}
+}}               }}                                          {% endif %}
+                                                             {{_('Download')}}
 
 {%- endmacro %} {% macro lom_file_list_box(files, pid, is_preview, record) %}
 {{ _("Files") }} {% if files %} ({{files|sum
-(attribute='size')|filesizeformat}}){% endif %}
+(attribute='size')|filesizeformat}}) {% endif %}
 {% if record.access.files == 'restricted' %}
-{{ record.ui.access_status.title_l10n }}
+ {{ record.ui.access_status.title_l10n }}
 {{ record.ui.access_status.description_l10n }}
 {% if record.access.embargo.reason %}
 {{_("Reason")}}: {{record.access.embargo.reason}}
 {% endif%}
 {% endif %}
 {{ file_list(files, pid, is_preview) }}
 {%- endmacro %}
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/records/macros/tree.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/search.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/search.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/templates/invenio_records_lom/uploads.html` & `invenio-records-lom-0.9.0/invenio_records_lom/templates/invenio_records_lom/uploads.html`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/translations/de/LC_MESSAGES/messages.po` & `invenio-records-lom-0.9.0/invenio_records_lom/translations/de/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 # project.
 #  <christoph.ladurner@tugraz.at>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: invenio_records_lom 0.1.0\n"
 "Report-Msgid-Bugs-To: info@tugraz.at\n"
-"POT-Creation-Date: 2023-04-28 13:37+0200\n"
-"PO-Revision-Date: 2023-04-28 13:37+0200\n"
+"POT-Creation-Date: 2023-05-09 10:59+0200\n"
+"PO-Revision-Date: 2023-05-09 11:01+0200\n"
 "Last-Translator: christoph.ladurner@tugraz.at\n"
 "Language-Team: Deutsch\n"
 "Language: de_AT\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.9.1\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
-"X-Generator: Poedit 2.3.1\n"
+"Generated-By: Babel 2.9.1\n"
+"X-Generator: Poedit 3.2.2\n"
 
 #: invenio_records_lom/config.py:23
 msgid "Best match"
 msgstr ""
 
 #: invenio_records_lom/config.py:27
 msgid "Newest"
@@ -124,23 +124,31 @@
 "Um die Upload-Funktion nutzen zu können, lassen Sie sich freischalten, indem "
 "Sie Ihr OER-Zertifikat „OER Practitioner\n"
 "        | OER-Praktiker:in“ der nationalen Zertifizierungsstelle an <a "
 "href=\"mailto:telucation@tugraz.at\">telucation@tugraz.at</a>\n"
 "        schicken."
 
 #: invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html:51
+#, fuzzy
+#| msgid ""
+#| "Not yet certified? Members of Graz University of Technology are required "
+#| "to obtain the OER certificate from\n"
+#| "        fnma at Graz University of Technology, which you can obatin as "
+#| "part of the in-house training. Please register\n"
+#| "        via your business card in <a href=\"online.tugraz."
+#| "at\">TUGRAZonline</a>."
 msgid ""
 "Not yet certified? Members of Graz University of Technology are required to "
 "obtain the OER certificate from\n"
-"        fnma at Graz University of Technology, which you can obatin as part "
+"        fnma at Graz University of Technology, which you can obtain as part "
 "of the in-house training. Please register\n"
 "        via your business card in <a href=\"online.tugraz.at\">TUGRAZonline</"
 "a>."
 msgstr ""
-" Noch nicht zertifiziert? Angehörige der TU Graz können das Zertifikat durch "
+"Noch nicht zertifiziert? Angehörige der TU Graz können das Zertifikat durch "
 "Teilnahme bei der der internen\n"
 "        Weiterbildung  OER-Zertifikats von fnma bei der TU Graz  erlangen. "
 "Bitte melden Sie sich über Ihre Visitenkarte im\n"
 "        TUGRAZonline dazu an."
 
 #: invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html:57
 msgid ""
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/translations/en/LC_MESSAGES/messages.po` & `invenio-records-lom-0.9.0/invenio_records_lom/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/translations/messages.pot` & `invenio-records-lom-0.9.0/invenio_records_lom/translations/messages.pot`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 # This file is distributed under the same license as the invenio-records-lom
 # project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: invenio-records-lom 0.8.0\n"
+"Project-Id-Version: invenio-records-lom 0.8.1\n"
 "Report-Msgid-Bugs-To: info@tugraz.at\n"
-"POT-Creation-Date: 2023-04-28 13:37+0200\n"
+"POT-Creation-Date: 2023-05-09 09:45+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Generated-By: Babel 2.12.1\n"
@@ -98,15 +98,15 @@
 "href=\"mailto:telucation@tugraz.at\">telucation@tugraz.at</a>."
 msgstr ""
 
 #: invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html:51
 msgid ""
 "Not yet certified? Members of Graz University of Technology are required "
 "to obtain the OER certificate from\n"
-"        fnma at Graz University of Technology, which you can obatin as "
+"        fnma at Graz University of Technology, which you can obtain as "
 "part of the in-house training. Please register\n"
 "        via your business card in <a "
 "href=\"online.tugraz.at\">TUGRAZonline</a>."
 msgstr ""
 
 #: invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html:57
 msgid ""
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/records/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/decorators.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/records/decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,29 @@
 # copy-pasting was necessary to overrride the standard-service with this module's service
 
 
 """Decorates for record-view-functions."""
 
 from functools import wraps
 
-from flask import g, request
+from flask import g, redirect, request, url_for
 from invenio_records_resources.services.errors import PermissionDeniedError
 from sqlalchemy.orm.exc import NoResultFound
 
 from ...proxies import current_records_lom
 
 
-# TODO: this implementation is a quick hack. it is a workflow of the tu graz and
-# should be implemented within the invenio-workflows-tugraz package
-def license_required(func: callable):
+def pass_is_oer_certified(func: callable):
     """Check if the logged in user has the permission to create oer's."""
 
     @wraps(func)
     def decoed(**kwargs):
-        # TODO: for now default false. implement proper check
-        kwargs["is_licensed"] = False
-        return func(**kwargs)
+        service = current_records_lom.records_service
+        is_oer_certified = service.check_permission(g.identity, "handle_oer")
+        return func(**kwargs, is_oer_certified=is_oer_certified)
 
     return decoed
 
 
 def pass_record_latest(func: callable):
     """Retrieve latest version of `record` from db and pass that into decorated function."""
 
@@ -218,7 +216,29 @@
             )
         except PermissionDeniedError:
             draft_files = None
 
         return func(**kwargs, draft_files=draft_files)
 
     return decoed
+
+
+def require_lom_permission(action_name: str, *, default_endpoint: str):
+    """Require permission from permission-policy, otherwise redirect to `default_endpoint`.
+
+    example usage:
+    @require_lom_permission('create', 'invenio_records_lom.uploads')
+    # checks `flask.g.identity` against `LOMPermissionPolicy.can_create`
+    # if no permission redirects to endpoint "uploads" of blueprint "invenio_records_lom"
+    """
+
+    def view_decorator(view_func):
+        @wraps(view_func)
+        def decorated_view(*args, **kwargs):
+            service = current_records_lom.records_service
+            if not service.check_permission(g.identity, action_name):
+                return redirect(url_for(default_endpoint))
+            return view_func(*args, **kwargs)
+
+        return decorated_view
+
+    return view_decorator
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/errors.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/records/errors.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/records/records.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/records/records.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # copy-pasting was necessary to overrride the standard-behavior with custom behavior
 
 """View-functions for record-related pages."""
 
 import typing as t
 from os.path import splitext
 
-from bs4 import BeautifulSoup
 from flask import abort, current_app, g, redirect, render_template, request, url_for
 from invenio_base.utils import obj_or_import_string
 from invenio_previewer.extensions import default
 from invenio_previewer.proxies import current_previewer
 from invenio_records_resources.services.files.results import FileItem, FileList
 from invenio_records_resources.services.records.results import RecordItem
 from marshmallow import ValidationError
@@ -98,57 +97,54 @@
     is_draft = record_ui["is_draft"]
     if is_preview and is_draft:
         try:
             current_records_lom.records_service.validate_draft(g.identity, record.id)
         except ValidationError:
             abort(404)
 
-    ugly_html_text = render_template(
+    return render_template(
         "invenio_records_lom/record.html",
         record=record_ui,
         pid=pid_value,
         files=files_dict,
         permissions=record.has_permissions_to(
             ["edit", "new_version", "manage", "update_draft", "read_files", "review"]
         ),
         is_preview=is_preview,
         is_draft=is_draft,
     )
-    return BeautifulSoup(ugly_html_text, features="lxml").prettify()
 
 
 @pass_is_preview
 @pass_record_or_draft
 def record_export(
     record: RecordItem = None,
     export_format: str = None,
-    pid_value: str = None,  # pylint: disable=unused-argument
-    is_preview: bool = False,
+    pid_value: str = None,
+    is_preview: bool = False,  # pylint: disable=unused-argument
 ):
     """Export view for LOM records."""
     exporter = current_app.config.get("LOM_RECORD_EXPORTERS", {}).get(export_format)
     if exporter is None:
         abort(404)
 
     serializer = obj_or_import_string(exporter["serializer"])(
         options={
             "indent": 2,
             "sort_keys": True,
         }
     )
     exported_record = serializer.serialize_object(record.to_dict())
-    return render_template(
-        "invenio_records_lom/records/export.html",
-        export_format=exporter.get("name", export_format),
-        exported_record=exported_record,
-        record=LOMUIJSONSerializer().serialize_object_to_dict(record.to_dict()),
-        permissions=record.has_permissions_to(["update_draft"]),
-        is_preview=is_preview,
-        is_draft=record._record.is_draft,  # pylint: disable=protected-access
-    )
+    content_type = exporter.get("content-type", export_format)
+    filename = exporter.get("filename", export_format).format(id=pid_value)
+    headers = {
+        "Content-Type": content_type,
+        "Content-Disposition": f"attachment; filename={filename}",
+    }
+    return (exported_record, 200, headers)
 
 
 @pass_is_preview
 @pass_record_or_draft
 @pass_file_metadata
 def record_file_preview(
     record: RecordItem = None,  # pylint: disable=unused-argument
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/LOMDepositForm.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -103,14 +103,16 @@
                 {
                     // TODO:
                     // uses paths of length two for now
                     // this works for now, as every category has only one sub-field that can have errors
                     // use longer paths once implemented in invenio...
                     "metadata.general": i18next.t("Title"),
                     "metadata.lifecycle": i18next.t("Contributors"),
+                    "metadata.technical": i18next.t("Format"),
+                    "metadata.educational": i18next.t("Resource Type"),
                     "metadata.rights": i18next.t("License"),
                     "metadata.classification": i18next.t("OEFOS"),
                 }
             }
             /> {
                 /* TODO: Community-Header */ } <
             Container id = "deposit-form"
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/components.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -145,14 +145,36 @@
         }
         required title = {
             i18next.t("License")
         }
         vocabularyName = "license" /
         >
         <
+        DropdownField fieldPath = "metadata.form.format"
+        iconName = "tag"
+        placeholder = {
+            i18next.t("Select Format")
+        }
+        required title = {
+            i18next.t("Format")
+        }
+        vocabularyName = "format" /
+        >
+        <
+        DropdownField fieldPath = "metadata.form.resourcetype"
+        iconName = "tag"
+        placeholder = {
+            i18next.t("Select Resource Type")
+        }
+        required title = {
+            i18next.t("Resource Type")
+        }
+        vocabularyName = "resourcetype" /
+        >
+        <
         ArrayField addButtonLabel = {
             i18next.t("Add Contributor")
         }
         defaultNewValue = {
             {}
         }
         fieldPath = "metadata.form.contributor"
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -219,14 +219,24 @@
         form.title = _get(metadata, "general.title.langstring.#text", "");
 
         // deserialize license
         form.license = {
             value: _get(metadata, "rights.url", "")
         };
 
+        // deserialize format
+        form.format = {
+            value: _get(metadata, "technical.format.0", "")
+        };
+
+        // deserialize resource-type
+        form.resourcetype = {
+            value: _get(metadata, "educational.learningresourcetype.id", ""),
+        };
+
         // deserialize contributors
         const validRoles = Object.keys(_get(this, "vocabularies.contributor", {}));
         form.contributor = [];
         for (const contribute of _get(metadata, "lifecycle.contribute", [])) {
             let role = _get(contribute, "role.value.langstring.#text", "");
             role = validRoles.includes(role) ? role : "";
             for (const name of contribute.entity || []) {
@@ -301,14 +311,37 @@
                 langstring: {
                     "#text": licenseUrl,
                     lang: "x-t-cc-url",
                 },
             },
         });
 
+        // serialize format
+        const format = _get(metadata, "form.format.value", "");
+        _set(metadata, "technical.format.0", format);
+
+        // set location
+        _set(
+            metadata,
+            "technical.location.#text",
+            _get(recordToSerialize, "links.record_html", "")
+        );
+
+        // serialize resource-type
+        const resourcetypeUrl = _get(metadata, "form.resourcetype.value");
+        _set(metadata, "educational.learningresourcetype", {
+            source: {
+                langstring: {
+                    "#text": "https://w3id.org/kim/hcrt/scheme",
+                    lang: "x-none",
+                },
+            },
+            id: resourcetypeUrl,
+        });
+
         // serialize contributors
         this.serializeContributor(recordToSerialize);
 
         // serialize oefos
         this.serializeOefos(recordToSerialize);
 
         // serialize description
@@ -382,18 +415,44 @@
             of errors) {
             if (String(field).startsWith("metadata.rights")) {
                 licenseErrorMessages.push(...messages);
             }
         }
         const licenseErrorMessage = licenseErrorMessages.join(" ");
         if (licenseErrorMessage) {
+            _set(deserializedErrors, "metadata.form.license", licenseErrorMessage);
+        }
+
+        // deserialize error for format
+        const formatErrorMessages = [];
+        for (const {
+                field,
+                messages
+            }
+            of errors) {
+            if (String(field).startsWith("metadata.technical.format")) {
+                formatErrorMessages.push(...messages);
+            }
+        }
+        const formatErrorMessage = formatErrorMessages.join(" ");
+        if (formatErrorMessage) {
+            _set(deserializedErrors, "metadata.form.format", formatErrorMessage);
+        }
+
+        // deserialize error for resourcetype
+        const resourcetypeErrorMessage = _get(
+            deserializedErrors,
+            "metadata.educational.learningresourcetype.id",
+            null
+        );
+        if (resourcetypeErrorMessage) {
             _set(
                 deserializedErrors,
-                "metadata.form.license",
-                licenseErrorMessages.join(" ")
+                "metadata.form.resourcetype",
+                resourcetypeErrorMessage
             );
         }
 
         // deserialize error for contribute
         const contributeError = _get(
             deserializedErrors,
             "metadata.lifecycle.contribute",
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/config.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/config.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/views.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/views.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/ui/theme/webpack.py` & `invenio-records-lom-0.9.0/invenio_records_lom/ui/theme/webpack.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv` & `invenio-records-lom-0.9.0/invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv` & `invenio-records-lom-0.9.0/invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/utils/__init__.py` & `invenio-records-lom-0.9.0/invenio_records_lom/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/utils/learning_resource_types.json` & `invenio-records-lom-0.9.0/invenio_records_lom/utils/learning_resource_types.json`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/utils/util.py` & `invenio-records-lom-0.9.0/invenio_records_lom/utils/util.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom/views.py` & `invenio-records-lom-0.9.0/invenio_records_lom/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     # Invenio-Records-Resources might not have been initialized.
     registry = app.extensions["invenio-records-resources"].registry
     ext = app.extensions["invenio-records-lom"]
 
     registry.register(ext.records_service, service_id="lom-records")
     registry.register(ext.records_service.files, service_id="lom-files")
     registry.register(ext.records_service.draft_files, service_id="lom-draft-files")
+    registry.register(ext.iiif_service, service_id="lom-iiif")
 
 
 def create_records_bp(app: Flask):
     """Create records blueprint."""
     ext = app.extensions["invenio-records-lom"]
     return ext.records_resource.as_blueprint()
 
@@ -39,7 +40,13 @@
     return ext.draft_files_resource.as_blueprint()
 
 
 def create_record_files_bp(app: Flask):
     """Create record files bluprint."""
     ext = app.extensions["invenio-records-lom"]
     return ext.record_files_resource.as_blueprint()
+
+
+def create_iiif_bp(app: Flask):
+    """Create IIIF blueprint."""
+    ext = app.extensions["invenio-records-lom"]
+    return ext.iiif_resource.as_blueprint()
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/PKG-INFO` & `invenio-records-lom-0.9.0/invenio_records_lom.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-records-lom
-Version: 0.8.1
+Version: 0.9.0
 Summary: "Invenio data model for Learning Object Metadata."
 Home-page: https://github.com/tu-graz-library/invenio-records-lom
 Author: "Graz University of Technology"
 Author-email: info@tugraz.at
 License: MIT
 Keywords: invenio record LOM learning object metadata
 Platform: any
@@ -45,28 +45,39 @@
         
 .. image:: https://readthedocs.org/projects/invenio-records-lom/badge/?version=latest
         :target: https://invenio-records-lom.readthedocs.io/en/latest/?badge=latest
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
         :target: https://github.com/psf/black
 
-invenio data model for Learning object metadata
+Invenio module that adds a data model based on LOM (Learning Object Metadata).
+The specification of the LOM-dialect used by this module can be found here: `LOM-UIBK (only available in german) <https://oer-repo.uibk.ac.at/lom/latest/>`_
 
 Further documentation is available on
 https://invenio-records-lom.readthedocs.io/
 
 ..
     Copyright (C) 2020 Graz University of Technology.
 
     invenio-records-lom is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
+Version v0.9.0 (release 2023-06-01)
+
+- add `format` and `resource-type` to upload-page
+- add schema for cleaner OAI-PMH-output
+- add "$schema"-key to jsons in database
+- update landing page
+- implement and configure permissions
+- fix image-preview by implementing iiif-resource
+
+
 Version v0.8.1 (release 2023-04-28)
 
 - upload: require license permission
 
 
 Version v0.8.0 (release 2023-04-20)
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/SOURCES.txt` & `invenio-records-lom-0.9.0/invenio_records_lom.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -39,14 +39,15 @@
 invenio_records_lom.egg-info/not-zip-safe
 invenio_records_lom.egg-info/requires.txt
 invenio_records_lom.egg-info/top_level.txt
 invenio_records_lom/fixtures/__init__.py
 invenio_records_lom/fixtures/demo.py
 invenio_records_lom/jsonschemas/__init__.py
 invenio_records_lom/jsonschemas/lomrecords/lom-v1.0.0.json
+invenio_records_lom/jsonschemas/lomrecords/records/record-v1.0.0.json
 invenio_records_lom/records/__init__.py
 invenio_records_lom/records/api.py
 invenio_records_lom/records/models.py
 invenio_records_lom/records/mappings/__init__.py
 invenio_records_lom/records/mappings/os-v2/__init__.py
 invenio_records_lom/records/mappings/os-v2/lomrecords/drafts/draft-v1.0.0.json
 invenio_records_lom/records/mappings/os-v2/lomrecords/records/record-v1.0.0.json
@@ -56,22 +57,29 @@
 invenio_records_lom/records/systemfields/relations.py
 invenio_records_lom/records/systemfields/resolver.py
 invenio_records_lom/records/systemfields/results.py
 invenio_records_lom/resources/__init__.py
 invenio_records_lom/resources/config.py
 invenio_records_lom/resources/resources.py
 invenio_records_lom/resources/serializers/__init__.py
-invenio_records_lom/resources/serializers/schemas.py
+invenio_records_lom/resources/serializers/schemas/__init__.py
+invenio_records_lom/resources/serializers/schemas/datacite.py
+invenio_records_lom/resources/serializers/schemas/oai.py
+invenio_records_lom/resources/serializers/schemas/ui.py
+invenio_records_lom/resources/serializers/schemas/utils.py
 invenio_records_lom/services/__init__.py
 invenio_records_lom/services/components.py
 invenio_records_lom/services/config.py
-invenio_records_lom/services/permissions.py
 invenio_records_lom/services/pids.py
 invenio_records_lom/services/services.py
 invenio_records_lom/services/tasks.py
+invenio_records_lom/services/permissions/__init__.py
+invenio_records_lom/services/permissions/generators.py
+invenio_records_lom/services/permissions/policy.py
+invenio_records_lom/services/permissions/roles.py
 invenio_records_lom/services/schemas/__init__.py
 invenio_records_lom/services/schemas/fields.py
 invenio_records_lom/services/schemas/metadata.py
 invenio_records_lom/services/schemas/records.py
 invenio_records_lom/static/templates/invenio_records_lom/results.html
 invenio_records_lom/templates/invenio_records_lom/base.html
 invenio_records_lom/templates/invenio_records_lom/not_licensed_text.html
@@ -101,14 +109,16 @@
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/debug.js
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/fields.js
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/index.js
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/deposit/serializers.js
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/components.js
 invenio_records_lom/ui/theme/assets/semantic-ui/js/invenio_records_lom/search/index.js
 invenio_records_lom/ui/theme/assets/semantic-ui/less/invenio_records_lom/theme.less
+invenio_records_lom/upgrade_scripts/__init__.py
+invenio_records_lom/upgrade_scripts/migrate_0_8_to_0_9.py
 invenio_records_lom/utils/OEFOS2012_DE_CTI_20211111_154218_utf8.csv
 invenio_records_lom/utils/OEFOS2012_EN_CTI_20211111_154228_utf8.csv
 invenio_records_lom/utils/__init__.py
 invenio_records_lom/utils/learning_resource_types.json
 invenio_records_lom/utils/util.py
 tests/conftest.py
 tests/test_cli.py
```

### Comparing `invenio-records-lom-0.8.1/invenio_records_lom.egg-info/entry_points.txt` & `invenio-records-lom-0.9.0/invenio_records_lom.egg-info/entry_points.txt`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 invenio_records_lom_theme = invenio_records_lom.ui.theme.webpack:theme
 
 [invenio_base.api_apps]
 invenio_records_lom = invenio_records_lom:InvenioRecordsLOM
 
 [invenio_base.api_blueprints]
 invenio_records_lom_draft_files = invenio_records_lom.views:create_draft_files_bp
+invenio_records_lom_iiif = invenio_records_lom.views:create_iiif_bp
 invenio_records_lom_record_files = invenio_records_lom.views:create_record_files_bp
 invenio_records_lom_records = invenio_records_lom.views:create_records_bp
 invenio_records_lom_resource_registerer = invenio_records_lom.views:blueprint
 
 [invenio_base.apps]
 invenio_records_lom = invenio_records_lom:InvenioRecordsLOM
```

### Comparing `invenio-records-lom-0.8.1/run-tests.sh` & `invenio-records-lom-0.9.0/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/setup.cfg` & `invenio-records-lom-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 	lom = invenio_records_lom.cli:lom
 invenio_assets.webpack = 
 	invenio_records_lom_theme = invenio_records_lom.ui.theme.webpack:theme
 invenio_base.api_apps = 
 	invenio_records_lom = invenio_records_lom:InvenioRecordsLOM
 invenio_base.api_blueprints = 
 	invenio_records_lom_draft_files = invenio_records_lom.views:create_draft_files_bp
+	invenio_records_lom_iiif = invenio_records_lom.views:create_iiif_bp
 	invenio_records_lom_record_files = invenio_records_lom.views:create_record_files_bp
 	invenio_records_lom_records = invenio_records_lom.views:create_records_bp
 	invenio_records_lom_resource_registerer = invenio_records_lom.views:blueprint
 invenio_base.apps = 
 	invenio_records_lom = invenio_records_lom:InvenioRecordsLOM
 invenio_base.blueprints = 
 	invenio_records_lom_ui = invenio_records_lom.ui:create_blueprint
```

### Comparing `invenio-records-lom-0.8.1/tests/conftest.py` & `invenio-records-lom-0.9.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 
 from invenio_records_lom.fixtures import create_fake_data
 
 
 @pytest.fixture(scope="module")
 def app_config(app_config):  # pylint: disable=redefined-outer-name
     """Override pytest-invenio app_config-fixture."""
+    # configuration for `jsonresolver`-package interoperability
+    app_config[
+        "RECORDS_REFRESOLVER_CLS"
+    ] = "invenio_records.resolver.InvenioRefResolver"
+    app_config[
+        "RECORDS_REFRESOLVER_STORE"
+    ] = "invenio_jsonschemas.proxies.current_refresolver_store"
+
     # Enable DOI minting...
     app_config["DATACITE_ENABLED"] = True
     app_config["DATACITE_USERNAME"] = "INVALID"
     app_config["DATACITE_PASSWORD"] = "INVALID"
     app_config["DATACITE_PREFIX"] = "10.1234"
     # ...but fake it
```

### Comparing `invenio-records-lom-0.8.1/tests/test_cli.py` & `invenio-records-lom-0.9.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/tests/test_invenio_records_lom.py` & `invenio-records-lom-0.9.0/tests/test_invenio_records_lom.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/tests/test_pids_service.py` & `invenio-records-lom-0.9.0/tests/test_pids_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/tests/test_service.py` & `invenio-records-lom-0.9.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `invenio-records-lom-0.8.1/tests/test_utils.py` & `invenio-records-lom-0.9.0/tests/test_utils.py`

 * *Files identical despite different names*

