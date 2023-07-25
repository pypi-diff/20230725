# Comparing `tmp/document_merge_service-6.2.2.tar.gz` & `tmp/document_merge_service-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_merge_service-6.2.2.tar", max compression
+gzip compressed data, was "document_merge_service-6.3.0.tar", max compression
```

## Comparing `document_merge_service-6.2.2.tar` & `document_merge_service-6.3.0.tar`

### file list

```diff
@@ -1,72 +1,71 @@
--rw-r--r--   0        0        0    11721 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/LICENSE
--rw-r--r--   0        0        0     2243 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/README.md
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/__init__.py
--rw-r--r--   0        0        0      405 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/apps.py
--rw-r--r--   0        0        0     3159 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/authentication.py
--rw-r--r--   0        0        0      504 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/__init__.py
--rw-r--r--   0        0        0      559 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/black.png
--rw-r--r--   0        0        0     9125 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge-syntax.docx
--rw-r--r--   0        0        0    11489 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge.docx
--rw-r--r--   0        0        0     5735 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-filters.docx
--rw-r--r--   0        0        0     6087 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-loopcontrols.docx
--rw-r--r--   0        0        0     5952 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-placeholdercheck.docx
--rw-r--r--   0        0        0     5091 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template-syntax.docx
--rw-r--r--   0        0        0     5490 2023-07-24 09:43:27.598401 document_merge_service-6.2.2/document_merge_service/api/data/docx-template.docx
--rw-r--r--   0        0        0  1127936 2023-07-24 09:43:27.602401 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/1.doc
--rw-r--r--   0        0        0   175922 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/2.docx
--rw-r--r--   0        0        0   163307 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/3.docx
--rw-r--r--   0        0        0   141498 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/loadtest/4.docx
--rw-r--r--   0        0        0       22 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/test.txt
--rw-r--r--   0        0        0        5 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-not-valid.xlsx
--rw-r--r--   0        0        0     6467 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-structure.xlsx
--rw-r--r--   0        0        0     6432 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-syntax.xlsx
--rw-r--r--   0        0        0     4750 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/data/xlsx-template.xlsx
--rw-r--r--   0        0        0     9772 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/engines.py
--rw-r--r--   0        0        0      389 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/factories.py
--rw-r--r--   0        0        0     2841 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/filters.py
--rw-r--r--   0        0        0     2546 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/jinja.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/__init__.py
--rw-r--r--   0        0        0     1628 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/clean_dangling_files.py
--rw-r--r--   0        0        0     1354 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/management/commands/upload_local_templates.py
--rw-r--r--   0        0        0     1248 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0001_initial.py
--rw-r--r--   0        0        0      488 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0002_template_group.py
--rw-r--r--   0        0        0      374 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0003_template_meta.py
--rw-r--r--   0        0        0      145 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0004_cleanup_files.py
--rw-r--r--   0        0        0     1004 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py
--rw-r--r--   0        0        0      932 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/0006_remove_template_group.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/migrations/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/models.py
--rw-r--r--   0        0        0      231 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/pagination.py
--rw-r--r--   0        0        0      289 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/permissions.py
--rw-r--r--   0        0        0     4651 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/serializers.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/__init__.py
--rw-r--r--   0        0        0    29399 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/snap_test_template.py
--rw-r--r--   0        0        0     2270 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_authentication.py
--rw-r--r--   0        0        0      942 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_clean_dangling_files.py
--rw-r--r--   0        0        0     1963 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_excel.py
--rw-r--r--   0        0        0     1372 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_filters.py
--rw-r--r--   0        0        0     1300 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_jinja.py
--rw-r--r--   0        0        0      749 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_pagination.py
--rw-r--r--   0        0        0    25634 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_template.py
--rw-r--r--   0        0        0     3425 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_unoconv.py
--rw-r--r--   0        0        0      597 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/tests/test_upload_local_templates.py
--rw-r--r--   0        0        0     6947 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/unoconv.py
--rw-r--r--   0        0        0      356 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/urls.py
--rw-r--r--   0        0        0     3570 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/api/views.py
--rw-r--r--   0        0        0     2909 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/conftest.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/__init__.py
--rw-r--r--   0        0        0       52 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/permissions.py
--rw-r--r--   0        0        0       52 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/extensions/visibilities.py
--rw-r--r--   0        0        0      789 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/sentry.py
--rw-r--r--   0        0        0     8818 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/settings.py
--rw-r--r--   0        0        0        0 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/__init__.py
--rw-r--r--   0        0        0      434 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/test_sentry.py
--rw-r--r--   0        0        0      615 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/tests/test_settings.py
--rw-r--r--   0        0        0      225 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/urls.py
--rw-r--r--   0        0        0      412 2023-07-24 09:43:27.606402 document_merge_service-6.2.2/document_merge_service/wsgi.py
--rw-r--r--   0        0        0     3571 2023-07-24 09:43:27.610401 document_merge_service-6.2.2/pyproject.toml
--rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11947 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/LICENSE
+-rw-r--r--   0        0        0     2243 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/__init__.py
+-rw-r--r--   0        0        0      405 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/apps.py
+-rw-r--r--   0        0        0     3159 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/authentication.py
+-rw-r--r--   0        0        0      504 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/black.png
+-rw-r--r--   0        0        0     9125 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge-syntax.docx
+-rw-r--r--   0        0        0    11489 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge.docx
+-rw-r--r--   0        0        0     5735 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-filters.docx
+-rw-r--r--   0        0        0     6087 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-loopcontrols.docx
+-rw-r--r--   0        0        0     5952 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-placeholdercheck.docx
+-rw-r--r--   0        0        0     5091 2023-07-25 08:52:57.507416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template-syntax.docx
+-rw-r--r--   0        0        0     5490 2023-07-25 08:52:57.511416 document_merge_service-6.3.0/document_merge_service/api/data/docx-template.docx
+-rw-r--r--   0        0        0  1127936 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/1.doc
+-rw-r--r--   0        0        0   175922 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/2.docx
+-rw-r--r--   0        0        0   163307 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/3.docx
+-rw-r--r--   0        0        0   141498 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/loadtest/4.docx
+-rw-r--r--   0        0        0       22 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/test.txt
+-rw-r--r--   0        0        0        5 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-not-valid.xlsx
+-rw-r--r--   0        0        0     6467 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-structure.xlsx
+-rw-r--r--   0        0        0     6432 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-syntax.xlsx
+-rw-r--r--   0        0        0     4750 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/data/xlsx-template.xlsx
+-rw-r--r--   0        0        0     9772 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/engines.py
+-rw-r--r--   0        0        0      389 2023-07-25 08:52:57.515416 document_merge_service-6.3.0/document_merge_service/api/factories.py
+-rw-r--r--   0        0        0     2841 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/filters.py
+-rw-r--r--   0        0        0     2546 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/jinja.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/__init__.py
+-rw-r--r--   0        0        0     1628 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/clean_dangling_files.py
+-rw-r--r--   0        0        0     1354 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/management/commands/upload_local_templates.py
+-rw-r--r--   0        0        0     1248 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0001_initial.py
+-rw-r--r--   0        0        0      488 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0002_template_group.py
+-rw-r--r--   0        0        0      374 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0003_template_meta.py
+-rw-r--r--   0        0        0      145 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0004_cleanup_files.py
+-rw-r--r--   0        0        0     1004 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py
+-rw-r--r--   0        0        0      932 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/0006_remove_template_group.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/migrations/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/models.py
+-rw-r--r--   0        0        0      231 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/pagination.py
+-rw-r--r--   0        0        0      289 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/permissions.py
+-rw-r--r--   0        0        0     4651 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/serializers.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/__init__.py
+-rw-r--r--   0        0        0    30689 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/__snapshots__/test_template.ambr
+-rw-r--r--   0        0        0     2270 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_authentication.py
+-rw-r--r--   0        0        0      942 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_clean_dangling_files.py
+-rw-r--r--   0        0        0     1963 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_excel.py
+-rw-r--r--   0        0        0     1372 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_filters.py
+-rw-r--r--   0        0        0     1300 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_jinja.py
+-rw-r--r--   0        0        0      749 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_pagination.py
+-rw-r--r--   0        0        0    25634 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_template.py
+-rw-r--r--   0        0        0     3425 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_unoconv.py
+-rw-r--r--   0        0        0      597 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/tests/test_upload_local_templates.py
+-rw-r--r--   0        0        0     6947 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/unoconv.py
+-rw-r--r--   0        0        0      356 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/urls.py
+-rw-r--r--   0        0        0     3570 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/api/views.py
+-rw-r--r--   0        0        0     2909 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/conftest.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/__init__.py
+-rw-r--r--   0        0        0       52 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/permissions.py
+-rw-r--r--   0        0        0       52 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/extensions/visibilities.py
+-rw-r--r--   0        0        0      789 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/sentry.py
+-rw-r--r--   0        0        0     8938 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/settings.py
+-rw-r--r--   0        0        0        0 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/__init__.py
+-rw-r--r--   0        0        0      434 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/test_sentry.py
+-rw-r--r--   0        0        0      615 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/tests/test_settings.py
+-rw-r--r--   0        0        0      225 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/urls.py
+-rw-r--r--   0        0        0      412 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/document_merge_service/wsgi.py
+-rw-r--r--   0        0        0     3555 2023-07-25 08:52:57.519416 document_merge_service-6.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4191 1970-01-01 00:00:00.000000 document_merge_service-6.3.0/PKG-INFO
```

### Comparing `document_merge_service-6.2.2/CHANGELOG.md` & `document_merge_service-6.3.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## 6.3.0 (25 July 2023)
+### Feature
+
+* **extensions:** Add setting for passing custom arguments into extensions ([`b76e293`](https://github.com/adfinis/document-merge-service/commit/b76e2930535f15820e449930e57d004c54e1ba2d))
+
 ## 6.2.2 (24 July 2023)
 ### Fix
 
 * **template:** Migrate group to meta property before removing ([`4480877`](https://github.com/adfinis/document-merge-service/commit/448087728f3103744b8245ff5400b63201352b19))
 
 ## 6.2.1 (19 July 2023)
 ### Fix
```

### Comparing `document_merge_service-6.2.2/LICENSE` & `document_merge_service-6.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/README.md` & `document_merge_service-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/authentication.py` & `document_merge_service-6.3.0/document_merge_service/api/authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/black.png` & `document_merge_service-6.3.0/document_merge_service/api/data/black.png`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge-syntax.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-mailmerge.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-mailmerge.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-filters.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-filters.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-loopcontrols.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-loopcontrols.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-placeholdercheck.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-placeholdercheck.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-template-syntax.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-template-syntax.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/docx-template.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/docx-template.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/1.doc` & `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/1.doc`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/2.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/2.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/3.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/3.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/loadtest/4.docx` & `document_merge_service-6.3.0/document_merge_service/api/data/loadtest/4.docx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-structure.xlsx` & `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-structure.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-syntax.xlsx` & `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-syntax.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/data/xlsx-template.xlsx` & `document_merge_service-6.3.0/document_merge_service/api/data/xlsx-template.xlsx`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/engines.py` & `document_merge_service-6.3.0/document_merge_service/api/engines.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/filters.py` & `document_merge_service-6.3.0/document_merge_service/api/filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/jinja.py` & `document_merge_service-6.3.0/document_merge_service/api/jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/management/commands/clean_dangling_files.py` & `document_merge_service-6.3.0/document_merge_service/api/management/commands/clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/management/commands/upload_local_templates.py` & `document_merge_service-6.3.0/document_merge_service/api/management/commands/upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/migrations/0001_initial.py` & `document_merge_service-6.3.0/document_merge_service/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/migrations/0005_xlsx_template_engine.py` & `document_merge_service-6.3.0/document_merge_service/api/migrations/0005_xlsx_template_engine.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/migrations/0006_remove_template_group.py` & `document_merge_service-6.3.0/document_merge_service/api/migrations/0006_remove_template_group.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/models.py` & `document_merge_service-6.3.0/document_merge_service/api/models.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/serializers.py` & `document_merge_service-6.3.0/document_merge_service/api/serializers.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/snapshots/snap_test_template.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/__snapshots__/test_template.ambr`

 * *Files 2% similar despite different names*

```diff
@@ -1,759 +1,764 @@
-# -*- coding: utf-8 -*-
-# snapshottest: v1 - https://goo.gl/zC4yUc
-from __future__ import unicode_literals
-
-from snapshottest import Snapshot
-
-
-snapshots = Snapshot()
-
-snapshots[
-    'test_merge_expression[{{NAME and ", represents " + NAME}}-template_content1] 1'
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test</w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">: , represents foo</w:t>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    'test_merge_expression[{{NAME and ", represents " + NAME}}-template_content2] 1'
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test</w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">: </w:t>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    "test_merge_expression[{{blah}}-template_content0] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test</w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">: blub</w:t>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    "test_merge_expression[{{escapeme}}-template_content3] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test</w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">: &lt;&amp;&gt;</w:t>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots["test_template_detail 1"] = {
-    "available_placeholders": None,
-    "description": """Article star very capital morning option. Interesting station story.
-Where during teach country talk across drop. Central meeting anyone remember. There today material minute ago get.""",
-    "disable_template_validation": False,
-    "engine": "docx-mailmerge",
-    "meta": {},
-    "sample_data": None,
-    "slug": "note-act-source",
-    "template": None,
-}
-
-snapshots[
-    "test_template_merge_docx[TestNameMailMerge-docx-mailmerge-template__template1] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:wpc="http://schemas.microsoft.com/office/word/2010/wordprocessingCanvas" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:m="http://schemas.openxmlformats.org/officeDocument/2006/math" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml" xmlns:w15="http://schemas.microsoft.com/office/word/2012/wordml" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:wpi="http://schemas.microsoft.com/office/word/2010/wordprocessingInk" xmlns:wne="http://schemas.microsoft.com/office/word/2006/wordml" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape">
-  <w:p w:rsidR="0083709B" w:rsidRPr="0083709B" w:rsidRDefault="0083709B">
-    <w:pPr>
-      <w:rPr>
-        <w:lang w:val="en-US"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="en-US"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test: </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="en-US"/>
-      </w:rPr>
-      <w:t>Test input</w:t>
-    </w:r>
-    <w:bookmarkStart w:id="0" w:name="_GoBack"/>
-    <w:bookmarkEnd w:id="0"/>
-  </w:p>
-  <w:sectPr w:rsidR="0083709B" w:rsidRPr="0083709B">
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:top="1417" w:right="1417" w:bottom="1134" w:left="1417" w:header="708" w:footer="708" w:gutter="0"/>
-    <w:cols w:space="708"/>
-    <w:docGrid w:linePitch="360"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    "test_template_merge_docx[TestNameTemplate-docx-template-template__template0] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">Test</w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">: Test input</w:t>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    "test_template_merge_jinja_extensions_docx[docx-template-template__template0] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="3E4349"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:ind w:left="0" w:right="0" w:hanging="0"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:ind w:left="0" w:right="0" w:hanging="0"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">    </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:i w:val="false"/>
-        <w:color w:val="B11414"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="3E4349"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve">    </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve">1</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="3E4349"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:ind w:left="0" w:right="0" w:hanging="0"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">    </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:i w:val="false"/>
-        <w:color w:val="B11414"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="3E4349"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve">    </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve">2</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="3E4349"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:ind w:left="0" w:right="0" w:hanging="0"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">    </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="PreformattedText"/>
-      <w:widowControl/>
-      <w:shd w:val="clear" w:fill="EEEEEE"/>
-      <w:spacing w:before="225" w:after="225"/>
-      <w:ind w:left="0" w:right="0" w:hanging="0"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve">        </w:t>
-    </w:r>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
-        <w:b w:val="false"/>
-        <w:i w:val="false"/>
-        <w:caps w:val="false"/>
-        <w:smallCaps w:val="false"/>
-        <w:color w:val="B11414"/>
-        <w:spacing w:val="0"/>
-        <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr/>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
-
-snapshots[
-    "test_template_merge_jinja_filters_docx[docx-template-template__template0-False-False-200] 1"
-] = """<w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">15.09.1984</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">1984</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">23:24</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">15.09.1984, 23:23:00</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">23:23</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">something</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve">This is</w:t>
-      <w:br/>
-      <w:t xml:space="preserve">a test.</w:t>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr/>
-    </w:pPr>
-    <w:r>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-      <w:t xml:space="preserve"/>
-    </w:r>
-    <w:r>
-      <w:drawing>
-        <wp:inline xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main" xmlns:pic="http://schemas.openxmlformats.org/drawingml/2006/picture">
-          <wp:extent cx="1800000" cy="1800000"/>
-          <wp:docPr id="1001" name="Picture 1"/>
-          <wp:cNvGraphicFramePr>
-            <a:graphicFrameLocks noChangeAspect="1"/>
-          </wp:cNvGraphicFramePr>
-          <a:graphic>
-            <a:graphicData uri="http://schemas.openxmlformats.org/drawingml/2006/picture">
-              <pic:pic>
-                <pic:nvPicPr>
-                  <pic:cNvPr id="0" name="image.png"/>
-                  <pic:cNvPicPr/>
-                </pic:nvPicPr>
-                <pic:blipFill>
-                  <a:blip r:embed="rId5"/>
-                  <a:stretch>
-                    <a:fillRect/>
-                  </a:stretch>
-                </pic:blipFill>
-                <pic:spPr>
-                  <a:xfrm>
-                    <a:off x="0" y="0"/>
-                    <a:ext cx="1800000" cy="1800000"/>
-                  </a:xfrm>
-                  <a:prstGeom prst="rect"/>
-                </pic:spPr>
-              </pic:pic>
-            </a:graphicData>
-          </a:graphic>
-        </wp:inline>
-      </w:drawing>
-    </w:r>
-    <w:r>
-      <w:t xml:space="preserve"/>
-    </w:r>
-  </w:p>
-  <w:p>
-    <w:pPr>
-      <w:pStyle w:val="Normal"/>
-      <w:rPr>
-        <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
-      </w:rPr>
-    </w:pPr>
-    <w:r>
-      <w:rPr/>
-    </w:r>
-  </w:p>
-  <w:sectPr>
-    <w:type w:val="nextPage"/>
-    <w:pgSz w:w="11906" w:h="16838"/>
-    <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
-    <w:pgNumType w:fmt="decimal"/>
-    <w:formProt w:val="false"/>
-    <w:textDirection w:val="lrTb"/>
-    <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
-  </w:sectPr>
-</w:body>
-"""
+# serializer version: 1
+# name: test_merge_expression[{{NAME and ", represents " + NAME}}-template_content1]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test</w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">: , represents foo</w:t>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_merge_expression[{{NAME and ", represents " + NAME}}-template_content2]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test</w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">: </w:t>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_merge_expression[{{blah}}-template_content0]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test</w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">: blub</w:t>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_merge_expression[{{escapeme}}-template_content3]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test</w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">: &lt;&amp;&gt;</w:t>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_template_detail
+  dict({
+    'available_placeholders': None,
+    'description': '''
+      Article star very capital morning option. Interesting station story.
+      Where during teach country talk across drop. Central meeting anyone remember. There today material minute ago get.
+    ''',
+    'disable_template_validation': False,
+    'engine': 'docx-mailmerge',
+    'meta': dict({
+    }),
+    'sample_data': None,
+    'slug': 'note-act-source',
+    'template': None,
+  })
+# ---
+# name: test_template_merge_docx[TestNameMailMerge-docx-mailmerge-template__template1]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:wpc="http://schemas.microsoft.com/office/word/2010/wordprocessingCanvas" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:m="http://schemas.openxmlformats.org/officeDocument/2006/math" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml" xmlns:w15="http://schemas.microsoft.com/office/word/2012/wordml" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:wpi="http://schemas.microsoft.com/office/word/2010/wordprocessingInk" xmlns:wne="http://schemas.microsoft.com/office/word/2006/wordml" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape">
+    <w:p w:rsidR="0083709B" w:rsidRPr="0083709B" w:rsidRDefault="0083709B">
+      <w:pPr>
+        <w:rPr>
+          <w:lang w:val="en-US"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="en-US"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test: </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="en-US"/>
+        </w:rPr>
+        <w:t>Test input</w:t>
+      </w:r>
+      <w:bookmarkStart w:id="0" w:name="_GoBack"/>
+      <w:bookmarkEnd w:id="0"/>
+    </w:p>
+    <w:sectPr w:rsidR="0083709B" w:rsidRPr="0083709B">
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:top="1417" w:right="1417" w:bottom="1134" w:left="1417" w:header="708" w:footer="708" w:gutter="0"/>
+      <w:cols w:space="708"/>
+      <w:docGrid w:linePitch="360"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_template_merge_docx[TestNameTemplate-docx-template-template__template0]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">Test</w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">: Test input</w:t>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_template_merge_jinja_extensions_docx[docx-template-template__template0]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="3E4349"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:ind w:left="0" w:right="0" w:hanging="0"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:ind w:left="0" w:right="0" w:hanging="0"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">    </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:i w:val="false"/>
+          <w:color w:val="B11414"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="3E4349"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve">    </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve">1</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="3E4349"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:ind w:left="0" w:right="0" w:hanging="0"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">    </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:i w:val="false"/>
+          <w:color w:val="B11414"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="3E4349"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve">    </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve">2</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="3E4349"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:ind w:left="0" w:right="0" w:hanging="0"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">    </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="PreformattedText"/>
+        <w:widowControl/>
+        <w:shd w:val="clear" w:fill="EEEEEE"/>
+        <w:spacing w:before="225" w:after="225"/>
+        <w:ind w:left="0" w:right="0" w:hanging="0"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve">        </w:t>
+      </w:r>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace" w:hAnsi="Consolas;Menlo;Deja Vu Sans Mono;Bitstream Vera Sans Mono;monospace"/>
+          <w:b w:val="false"/>
+          <w:i w:val="false"/>
+          <w:caps w:val="false"/>
+          <w:smallCaps w:val="false"/>
+          <w:color w:val="B11414"/>
+          <w:spacing w:val="0"/>
+          <w:lang w:val="de-CH" w:eastAsia="zh-CN" w:bidi="hi-IN"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr/>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
+# name: test_template_merge_jinja_filters_docx[docx-template-template__template0-False-False-200]
+  '''
+  <w:body xmlns:w="http://schemas.openxmlformats.org/wordprocessingml/2006/main" xmlns:o="urn:schemas-microsoft-com:office:office" xmlns:r="http://schemas.openxmlformats.org/officeDocument/2006/relationships" xmlns:v="urn:schemas-microsoft-com:vml" xmlns:w10="urn:schemas-microsoft-com:office:word" xmlns:wp="http://schemas.openxmlformats.org/drawingml/2006/wordprocessingDrawing" xmlns:wps="http://schemas.microsoft.com/office/word/2010/wordprocessingShape" xmlns:wpg="http://schemas.microsoft.com/office/word/2010/wordprocessingGroup" xmlns:mc="http://schemas.openxmlformats.org/markup-compatibility/2006" xmlns:wp14="http://schemas.microsoft.com/office/word/2010/wordprocessingDrawing" xmlns:w14="http://schemas.microsoft.com/office/word/2010/wordml">
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">15.09.1984</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">1984</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">23:24</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">15.09.1984, 23:23:00</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">23:23</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">something</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve">This is</w:t>
+        <w:br/>
+        <w:t xml:space="preserve">a test.</w:t>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr/>
+      </w:pPr>
+      <w:r>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+        <w:t xml:space="preserve"/>
+      </w:r>
+      <w:r>
+        <w:drawing>
+          <wp:inline xmlns:a="http://schemas.openxmlformats.org/drawingml/2006/main" xmlns:pic="http://schemas.openxmlformats.org/drawingml/2006/picture">
+            <wp:extent cx="1800000" cy="1800000"/>
+            <wp:docPr id="1001" name="Picture 1"/>
+            <wp:cNvGraphicFramePr>
+              <a:graphicFrameLocks noChangeAspect="1"/>
+            </wp:cNvGraphicFramePr>
+            <a:graphic>
+              <a:graphicData uri="http://schemas.openxmlformats.org/drawingml/2006/picture">
+                <pic:pic>
+                  <pic:nvPicPr>
+                    <pic:cNvPr id="0" name="image.png"/>
+                    <pic:cNvPicPr/>
+                  </pic:nvPicPr>
+                  <pic:blipFill>
+                    <a:blip r:embed="rId5"/>
+                    <a:stretch>
+                      <a:fillRect/>
+                    </a:stretch>
+                  </pic:blipFill>
+                  <pic:spPr>
+                    <a:xfrm>
+                      <a:off x="0" y="0"/>
+                      <a:ext cx="1800000" cy="1800000"/>
+                    </a:xfrm>
+                    <a:prstGeom prst="rect"/>
+                  </pic:spPr>
+                </pic:pic>
+              </a:graphicData>
+            </a:graphic>
+          </wp:inline>
+        </w:drawing>
+      </w:r>
+      <w:r>
+        <w:t xml:space="preserve"/>
+      </w:r>
+    </w:p>
+    <w:p>
+      <w:pPr>
+        <w:pStyle w:val="Normal"/>
+        <w:rPr>
+          <w:rFonts w:ascii="DejaVu Sans" w:hAnsi="DejaVu Sans"/>
+        </w:rPr>
+      </w:pPr>
+      <w:r>
+        <w:rPr/>
+      </w:r>
+    </w:p>
+    <w:sectPr>
+      <w:type w:val="nextPage"/>
+      <w:pgSz w:w="11906" w:h="16838"/>
+      <w:pgMar w:left="1134" w:right="1134" w:header="0" w:top="1134" w:footer="0" w:bottom="1134" w:gutter="0"/>
+      <w:pgNumType w:fmt="decimal"/>
+      <w:formProt w:val="false"/>
+      <w:textDirection w:val="lrTb"/>
+      <w:docGrid w:type="default" w:linePitch="240" w:charSpace="0"/>
+    </w:sectPr>
+  </w:body>
+  
+  '''
+# ---
```

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_authentication.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_clean_dangling_files.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_clean_dangling_files.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_excel.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_excel.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_filters.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_jinja.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_jinja.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_pagination.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_template.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_unoconv.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/tests/test_upload_local_templates.py` & `document_merge_service-6.3.0/document_merge_service/api/tests/test_upload_local_templates.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/unoconv.py` & `document_merge_service-6.3.0/document_merge_service/api/unoconv.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/api/views.py` & `document_merge_service-6.3.0/document_merge_service/api/views.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/conftest.py` & `document_merge_service-6.3.0/document_merge_service/conftest.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/sentry.py` & `document_merge_service-6.3.0/document_merge_service/sentry.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/document_merge_service/settings.py` & `document_merge_service-6.3.0/document_merge_service/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,7 +268,10 @@
         SENTRY_TRACES_SAMPLE_RATE,
         SENTRY_SEND_DEFAULT_PII,
     )
 
 # https://github.com/adfinis/django-generic-api-permissions
 GENERIC_PERMISSIONS_PERMISSION_CLASSES = env.list("DMS_PERMISSION_CLASSES", default=[])
 GENERIC_PERMISSIONS_VISIBILITY_CLASSES = env.list("DMS_VISIBILITY_CLASSES", default=[])
+
+# App specific arguments for the extension classes
+EXTENSIONS_ARGUMENTS = env.dict("EXTENSIONS_ARGUMENTS", default={})
```

### Comparing `document_merge_service-6.2.2/document_merge_service/tests/test_settings.py` & `document_merge_service-6.3.0/document_merge_service/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `document_merge_service-6.2.2/pyproject.toml` & `document_merge_service-6.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "document-merge-service"
-version = "6.2.2"
+version = "6.3.0"
 description = "Merge Document Template Service"
 license = "GPL-3.0-or-later"
 authors = ["Adfinis AG <info@adfinis.com>"]
 homepage = "https://github.com/adfinis/document-merge-service"
 repository = "https://github.com/adfinis/document-merge-service"
 documentation = "https://github.com/adfinis/document-merge-service/blob/main/README.md"
 readme = "README.md"
@@ -62,15 +62,15 @@
 pytest-django = "4.5.2"
 pytest-env = "0.8.2"
 pytest-factoryboy = "2.5.1"
 pytest-mock = "3.11.1"
 pytest-randomly = "3.13.0"
 python-semantic-release = "7.34.6"
 requests-mock = "1.11.0"
-snapshottest = "0.6.0"
+syrupy = "4.0.8"
 types-python-dateutil = "2.8.19.14"
 types-requests = "2.31.0.2"
 types-setuptools = "68.0.0.3"
 types-toml = "0.10.8.7"
 
 [tool.poetry.extras]
 mysql = ["mysqlclient"]
@@ -78,15 +78,15 @@
 databases = ["mysqlclient", "psycopg2-binary"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
-skip = "migrations,snapshots"
+skip = "migrations"
 known_first_party = "document_merge_service"
 multi_line_output = 3
 include_trailing_comma = true
 force_grid_wrap = 0
 combine_as_imports = true
 line_length = 88
```

### Comparing `document_merge_service-6.2.2/PKG-INFO` & `document_merge_service-6.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: document-merge-service
-Version: 6.2.2
+Version: 6.3.0
 Summary: Merge Document Template Service
 Home-page: https://github.com/adfinis/document-merge-service
 License: GPL-3.0-or-later
 Author: Adfinis AG
 Author-email: info@adfinis.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

