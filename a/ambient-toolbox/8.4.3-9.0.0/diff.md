# Comparing `tmp/ambient_toolbox-8.4.3.tar.gz` & `tmp/ambient_toolbox-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient_toolbox-8.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ambient_toolbox-9.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ambient_toolbox-8.4.3.tar` & `ambient_toolbox-9.0.0.tar`

### file list

```diff
@@ -1,221 +1,221 @@
--rw-r--r--   0        0        0     3010 2023-07-25 08:56:18.249796 ambient_toolbox-8.4.3/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-07-25 09:33:29.848256 ambient_toolbox-8.4.3/.coveragerc
--rw-r--r--   0        0        0      288 2023-07-25 09:33:29.863918 ambient_toolbox-8.4.3/.editorconfig
--rw-r--r--   0        0        0     1700 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/.gitignore
--rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-07-25 09:33:29.863918 ambient_toolbox-8.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-07-25 09:33:29.863918 ambient_toolbox-8.4.3/.readthedocs.yml
--rw-r--r--   0        0        0    19502 2023-07-25 09:37:38.697857 ambient_toolbox-8.4.3/CHANGES.md
--rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/Dockerfile
--rw-r--r--   0        0        0     1107 2023-07-25 09:33:29.863918 ambient_toolbox-8.4.3/LICENSE.md
--rw-r--r--   0        0        0      134 2023-07-25 09:33:29.863918 ambient_toolbox-8.4.3/MANIFEST.in
--rw-r--r--   0        0        0     5857 2023-07-25 09:33:29.879542 ambient_toolbox-8.4.3/README.md
--rw-r--r--   0        0        0      116 2023-07-25 09:37:38.697857 ambient_toolbox-8.4.3/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/admin/views/mixins.py
--rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/apps.py
--rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/context_manager.py
--rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/drf/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/drf/fields.py
--rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient_toolbox-8.4.3/ambient_toolbox/drf/serializers.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/drf/tests.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/graphql/tests/base_test.py
--rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mail/backends/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1789 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/management/commands/install_permission_fixtures.py
--rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/managers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/middleware/__init__.py
--rw-r--r--   0        0        0      919 2023-05-22 13:49:14.233333 ambient_toolbox-8.4.3/ambient_toolbox/middleware/current_request.py
--rw-r--r--   0        0        0     1005 2023-05-22 13:49:14.233333 ambient_toolbox-8.4.3/ambient_toolbox/middleware/current_user.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mixins/models.py
--rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/mixins/validation.py
--rw-r--r--   0        0        0     3059 2023-07-24 07:16:28.327415 ambient_toolbox-8.4.3/ambient_toolbox/models.py
--rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0      307 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/permissions/fixtures/declarations.py
--rw-r--r--   0        0        0      242 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/permissions/fixtures/helpers.py
--rw-r--r--   0        0        0     3189 2023-05-12 07:03:57.505757 ambient_toolbox-8.4.3/ambient_toolbox/permissions/fixtures/services.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/selectors/__init__.py
--rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/selectors/base.py
--rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/selectors/permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/sentry/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-16 08:19:30.991454 ambient_toolbox-8.4.3/ambient_toolbox/sentry/helpers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/services/__init__.py
--rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/tests/__init__.py
--rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/tests/errors.py
--rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient_toolbox-8.4.3/ambient_toolbox/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/date.py
--rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/file.py
--rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/math.py
--rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/model.py
--rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/named_tuple.py
--rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/utils/string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/ambient_toolbox/view_layer/views.py
--rw-r--r--   0        0        0      654 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/docs/Makefile
--rw-r--r--   0        0        0     2803 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/docs/conf.py
--rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/admin.md
--rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/context_manager.md
--rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/gitlab.md
--rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient_toolbox-8.4.3/docs/features/graphql.md
--rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/mixins.md
--rw-r--r--   0        0        0     1556 2023-05-22 13:49:14.235382 ambient_toolbox-8.4.3/docs/features/models.md
--rw-r--r--   0        0        0     6340 2023-05-12 07:04:33.511067 ambient_toolbox-8.4.3/docs/features/permissions.md
--rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/selectors.md
--rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient_toolbox-8.4.3/docs/features/sentry.md
--rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/services.md
--rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/setup.md
--rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/tests.md
--rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils.rst
--rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/utils/string.md
--rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/docs/features/view-layer.md
--rw-r--r--   0        0        0     1185 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/manage.py
--rw-r--r--   0        0        0     4165 2023-07-25 09:33:29.879542 ambient_toolbox-8.4.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/pytest.ini
--rw-r--r--   0        0        0       56 2023-07-25 09:33:29.879542 ambient_toolbox-8.4.3/pytest.init
--rw-r--r--   0        0        0       50 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/scripts/publish_to_pypi.ps1
--rw-r--r--   0        0        0       50 2023-07-25 09:33:29.895129 ambient_toolbox-8.4.3/scripts/publish_to_pypi.sh
--rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient_toolbox-8.4.3/settings.py
--rw-r--r--   0        0        0       69 2023-07-25 09:33:29.879542 ambient_toolbox-8.4.3/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/forms.py
--rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/managers.py
--rw-r--r--   0        0        0     6221 2023-07-24 07:16:28.329010 ambient_toolbox-8.4.3/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3417 2023-07-24 07:16:28.329932 ambient_toolbox-8.4.3/testapp/models.py
--rw-r--r--   0        0        0      418 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/testapp/permissions.py
--rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/selectors.py
--rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/templates/testapp/test_template.html
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-8.4.3/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/testapp/urls.py
--rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/testapp/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/drf/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/drf/test_fields.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/mixins/validation.py
--rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0     1094 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/fixtures/test_declarations.py
--rw-r--r--   0        0        0      578 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/fixtures/test_helpers.py
--rw-r--r--   0        0        0     7227 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/fixtures/test_services_setup_service.py
--rw-r--r--   0        0        0      991 2023-05-12 07:03:57.521398 ambient_toolbox-8.4.3/tests/permissions/test_install_permission_fixtures_command.py
--rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/query_selectors/test_base.py
--rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/query_selectors/test_permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/selectors/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient_toolbox-8.4.3/tests/sentry/__init__.py
--rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient_toolbox-8.4.3/tests/sentry/mock_data.py
--rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient_toolbox-8.4.3/tests/sentry/test_sentry_helper.py
--rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_context_manager.py
--rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_log_whodid.py
--rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_managers.py
--rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_math.py
--rw-r--r--   0        0        0     4219 2023-05-22 13:49:14.236383 ambient_toolbox-8.4.3/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_mixins_models.py
--rw-r--r--   0        0        0     2130 2023-07-24 07:16:28.330933 ambient_toolbox-8.4.3/tests/test_models.py
--rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_utils_file.py
--rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient_toolbox-8.4.3/tests/test_utils_model.py
--rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient_toolbox-8.4.3/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     8273 1970-01-01 00:00:00.000000 ambient_toolbox-8.4.3/PKG-INFO
+-rw-r--r--   0        0        0     3010 2023-07-25 13:03:15.029874 ambient_toolbox-9.0.0/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-07-25 13:03:16.429108 ambient_toolbox-9.0.0/.coveragerc
+-rw-r--r--   0        0        0      288 2023-07-25 13:03:16.431120 ambient_toolbox-9.0.0/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-07-25 13:03:16.457881 ambient_toolbox-9.0.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/.gitignore
+-rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-07-25 13:03:16.432120 ambient_toolbox-9.0.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-07-25 13:03:16.434120 ambient_toolbox-9.0.0/.readthedocs.yml
+-rw-r--r--   0        0        0    19592 2023-07-25 13:01:44.672339 ambient_toolbox-9.0.0/CHANGES.md
+-rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-07-25 13:03:16.436120 ambient_toolbox-9.0.0/LICENSE.md
+-rw-r--r--   0        0        0      134 2023-07-25 13:03:16.437122 ambient_toolbox-9.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     5857 2023-07-25 13:03:16.453879 ambient_toolbox-9.0.0/README.md
+-rw-r--r--   0        0        0      116 2023-07-25 13:01:44.672339 ambient_toolbox-9.0.0/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/admin/views/mixins.py
+-rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/apps.py
+-rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/context_manager.py
+-rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/drf/fields.py
+-rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient_toolbox-9.0.0/ambient_toolbox/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/drf/tests.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     1789 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/management/commands/install_permission_fixtures.py
+-rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/managers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/middleware/__init__.py
+-rw-r--r--   0        0        0      919 2023-05-22 13:49:14.233333 ambient_toolbox-9.0.0/ambient_toolbox/middleware/current_request.py
+-rw-r--r--   0        0        0     1005 2023-05-22 13:49:14.233333 ambient_toolbox-9.0.0/ambient_toolbox/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mixins/models.py
+-rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/mixins/validation.py
+-rw-r--r--   0        0        0     3059 2023-07-24 07:16:28.327415 ambient_toolbox-9.0.0/ambient_toolbox/models.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/permissions/fixtures/declarations.py
+-rw-r--r--   0        0        0      242 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/permissions/fixtures/helpers.py
+-rw-r--r--   0        0        0     3189 2023-05-12 07:03:57.505757 ambient_toolbox-9.0.0/ambient_toolbox/permissions/fixtures/services.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/selectors/base.py
+-rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/selectors/permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/sentry/__init__.py
+-rw-r--r--   0        0        0     2164 2023-05-16 08:19:30.991454 ambient_toolbox-9.0.0/ambient_toolbox/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/services/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/tests/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/tests/errors.py
+-rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient_toolbox-9.0.0/ambient_toolbox/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/date.py
+-rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/file.py
+-rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/math.py
+-rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/model.py
+-rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/named_tuple.py
+-rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/utils/string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/ambient_toolbox/view_layer/views.py
+-rw-r--r--   0        0        0      654 2023-07-25 13:03:16.464938 ambient_toolbox-9.0.0/docs/Makefile
+-rw-r--r--   0        0        0     2803 2023-07-25 13:03:16.460410 ambient_toolbox-9.0.0/docs/conf.py
+-rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/admin.md
+-rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/context_manager.md
+-rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient_toolbox-9.0.0/docs/features/graphql.md
+-rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/mixins.md
+-rw-r--r--   0        0        0     1556 2023-05-22 13:49:14.235382 ambient_toolbox-9.0.0/docs/features/models.md
+-rw-r--r--   0        0        0     6340 2023-05-12 07:04:33.511067 ambient_toolbox-9.0.0/docs/features/permissions.md
+-rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/selectors.md
+-rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient_toolbox-9.0.0/docs/features/sentry.md
+-rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/services.md
+-rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/setup.md
+-rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils.rst
+-rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1185 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-07-25 13:03:16.462412 ambient_toolbox-9.0.0/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/manage.py
+-rw-r--r--   0        0        0     4083 2023-07-25 13:03:16.444378 ambient_toolbox-9.0.0/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/pytest.ini
+-rw-r--r--   0        0        0       56 2023-07-25 13:03:16.447357 ambient_toolbox-9.0.0/pytest.init
+-rw-r--r--   0        0        0       50 2023-07-25 13:03:16.466950 ambient_toolbox-9.0.0/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-07-25 13:03:16.467950 ambient_toolbox-9.0.0/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient_toolbox-9.0.0/settings.py
+-rw-r--r--   0        0        0       69 2023-07-25 13:03:16.455880 ambient_toolbox-9.0.0/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/forms.py
+-rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/managers.py
+-rw-r--r--   0        0        0     6221 2023-07-24 07:16:28.329010 ambient_toolbox-9.0.0/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3417 2023-07-24 07:16:28.329932 ambient_toolbox-9.0.0/testapp/models.py
+-rw-r--r--   0        0        0      418 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/testapp/permissions.py
+-rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/selectors.py
+-rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/templates/testapp/test_template.html
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient_toolbox-9.0.0/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/testapp/urls.py
+-rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/testapp/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/drf/test_fields.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/mixins/validation.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0     1094 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/fixtures/test_declarations.py
+-rw-r--r--   0        0        0      578 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/fixtures/test_helpers.py
+-rw-r--r--   0        0        0     7227 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/fixtures/test_services_setup_service.py
+-rw-r--r--   0        0        0      991 2023-05-12 07:03:57.521398 ambient_toolbox-9.0.0/tests/permissions/test_install_permission_fixtures_command.py
+-rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/query_selectors/test_base.py
+-rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/query_selectors/test_permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/selectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient_toolbox-9.0.0/tests/sentry/__init__.py
+-rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient_toolbox-9.0.0/tests/sentry/mock_data.py
+-rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient_toolbox-9.0.0/tests/sentry/test_sentry_helper.py
+-rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_context_manager.py
+-rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_log_whodid.py
+-rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_managers.py
+-rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_math.py
+-rw-r--r--   0        0        0     4219 2023-05-22 13:49:14.236383 ambient_toolbox-9.0.0/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     2130 2023-07-24 07:16:28.330933 ambient_toolbox-9.0.0/tests/test_models.py
+-rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_utils_file.py
+-rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient_toolbox-9.0.0/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient_toolbox-9.0.0/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     8195 1970-01-01 00:00:00.000000 ambient_toolbox-9.0.0/PKG-INFO
```

### Comparing `ambient_toolbox-8.4.3/.ambient-package-update/metadata.py` & `ambient_toolbox-9.0.0/.ambient-package-update/metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 * Install ambient-toolbox and remove the dependency to ai-django-core
 * Search and replace all usages of `from ai_django_core...` to `from ambient_toolbox...`
 * The class-based mail functionality was moved to a separate package called
 [django-pony-express](https://pypi.org/project/django-pony-express/).
 """,
     ),
     dependencies=[
-        'Django>=2.2.28',
+        'Django>=3.2.20',
         'bleach>=1.4,<6',
         'python-dateutil>=2.5.3',
     ],
     optional_dependencies={
         'dev': [
             *DEV_DEPENDENCIES,
             'gevent~=22.10',
```

### Comparing `ambient_toolbox-8.4.3/.github/workflows/ci.yml` & `ambient_toolbox-9.0.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/.gitignore` & `ambient_toolbox-9.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/.gitlab-ci.yml` & `ambient_toolbox-9.0.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/.pre-commit-config.yaml` & `ambient_toolbox-9.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/.readthedocs.yml` & `ambient_toolbox-9.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/CHANGES.md` & `ambient_toolbox-9.0.0/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+**9.0.0** (2023-07-25)
+  * Dropped support for deprecated Django versions 2.2, 3.1 & 4.0
+
 **8.4.3** (2023-07-25)
   * Updated linting and metadata
 
 **8.4.2** (2023-07-24)
   * Fixed a bug and a compatability issue with "django-safedelete" with `CommonInfo.save()`
 
 **8.4.1** (2023-07-17)
```

### Comparing `ambient_toolbox-8.4.3/Dockerfile` & `ambient_toolbox-9.0.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/LICENSE.md` & `ambient_toolbox-9.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/README.md` & `ambient_toolbox-9.0.0/README.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/classes.py` & `ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/inlines.py` & `ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/admin/model_admins/mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/admin/views/forms.py` & `ambient_toolbox-9.0.0/ambient_toolbox/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/admin/views/mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/context_manager.py` & `ambient_toolbox-9.0.0/ambient_toolbox/context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/drf/fields.py` & `ambient_toolbox-9.0.0/ambient_toolbox/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/drf/serializers.py` & `ambient_toolbox-9.0.0/ambient_toolbox/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/drf/tests.py` & `ambient_toolbox-9.0.0/ambient_toolbox/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/gitlab/coverage.py` & `ambient_toolbox-9.0.0/ambient_toolbox/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/graphql/forms/mutations.py` & `ambient_toolbox-9.0.0/ambient_toolbox/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/graphql/schemes/mutations.py` & `ambient_toolbox-9.0.0/ambient_toolbox/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/graphql/sentry/views.py` & `ambient_toolbox-9.0.0/ambient_toolbox/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/graphql/tests/base_test.py` & `ambient_toolbox-9.0.0/ambient_toolbox/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo` & `ambient_toolbox-9.0.0/ambient_toolbox/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po` & `ambient_toolbox-9.0.0/ambient_toolbox/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/mail/backends/whitelist_smtp.py` & `ambient_toolbox-9.0.0/ambient_toolbox/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/management/commands/install_permission_fixtures.py` & `ambient_toolbox-9.0.0/ambient_toolbox/management/commands/install_permission_fixtures.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/managers.py` & `ambient_toolbox-9.0.0/ambient_toolbox/managers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/middleware/current_request.py` & `ambient_toolbox-9.0.0/ambient_toolbox/middleware/current_request.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/middleware/current_user.py` & `ambient_toolbox-9.0.0/ambient_toolbox/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/mixins/bleacher.py` & `ambient_toolbox-9.0.0/ambient_toolbox/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/mixins/models.py` & `ambient_toolbox-9.0.0/ambient_toolbox/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/models.py` & `ambient_toolbox-9.0.0/ambient_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/permissions/fixtures/services.py` & `ambient_toolbox-9.0.0/ambient_toolbox/permissions/fixtures/services.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/selectors/permission.py` & `ambient_toolbox-9.0.0/ambient_toolbox/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/sentry/helpers.py` & `ambient_toolbox-9.0.0/ambient_toolbox/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/services/custom_scrubber.py` & `ambient_toolbox-9.0.0/ambient_toolbox/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_email_tags.py` & `ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_file_tags.py` & `ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_number_tags.py` & `ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/templatetags/ai_string_tags.py` & `ambient_toolbox-9.0.0/ambient_toolbox/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/tests/mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py` & `ambient_toolbox-9.0.0/ambient_toolbox/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/date.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/date.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/file.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/file.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/math.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/math.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/model.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/model.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/named_tuple.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/utils/string.py` & `ambient_toolbox-9.0.0/ambient_toolbox/utils/string.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/form_mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/formset_view_mixin.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/htmx_mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/tests/mixins.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/ambient_toolbox/view_layer/views.py` & `ambient_toolbox-9.0.0/ambient_toolbox/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/Makefile` & `ambient_toolbox-9.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/conf.py` & `ambient_toolbox-9.0.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/admin.md` & `ambient_toolbox-9.0.0/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/context_manager.md` & `ambient_toolbox-9.0.0/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/context_processors.md` & `ambient_toolbox-9.0.0/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/database_anonymisation.md` & `ambient_toolbox-9.0.0/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/djangorestframework.md` & `ambient_toolbox-9.0.0/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/gitlab.md` & `ambient_toolbox-9.0.0/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/graphql.md` & `ambient_toolbox-9.0.0/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/mail.md` & `ambient_toolbox-9.0.0/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/managers.md` & `ambient_toolbox-9.0.0/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/mixins.md` & `ambient_toolbox-9.0.0/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/models.md` & `ambient_toolbox-9.0.0/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/permissions.md` & `ambient_toolbox-9.0.0/docs/features/permissions.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/selectors.md` & `ambient_toolbox-9.0.0/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/sentry.md` & `ambient_toolbox-9.0.0/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/services.md` & `ambient_toolbox-9.0.0/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/setup.md` & `ambient_toolbox-9.0.0/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/tests.md` & `ambient_toolbox-9.0.0/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/cache.md` & `ambient_toolbox-9.0.0/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/date.md` & `ambient_toolbox-9.0.0/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/math.md` & `ambient_toolbox-9.0.0/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/model.md` & `ambient_toolbox-9.0.0/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/named_tuple.md` & `ambient_toolbox-9.0.0/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/utils/string.md` & `ambient_toolbox-9.0.0/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/features/view-layer.md` & `ambient_toolbox-9.0.0/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/index.rst` & `ambient_toolbox-9.0.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/docs/make.bat` & `ambient_toolbox-9.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/manage.py` & `ambient_toolbox-9.0.0/manage.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/pyproject.toml` & `ambient_toolbox-9.0.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,15 @@
     {'name' = 'Ambient Digital', 'email' = 'hello@ambient.digital'},
 ]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Framework :: Django",
-    "Framework :: Django :: 3.1",
     "Framework :: Django :: 3.2",
-    "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
@@ -28,15 +26,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Utilities",
 ]
 dynamic = ["version", "description"]
 license = {"file" = "LICENSE.md"}
 dependencies = [
-    'Django>=2.2.28',
+    'Django>=3.2.20',
     'bleach>=1.4,<6',
     'python-dateutil>=2.5.3',
 ]
 
 
 [project.optional-dependencies]
 dev = [
@@ -46,15 +44,15 @@
    'pre-commit~=3.2',
    'black~=23.3',
    'Django~=3.2',
    'sphinx==4.2.0',
    'sphinx-rtd-theme==1.0.0',
    'm2r2==0.3.1',
    'mistune<2.0.0',
-   'ambient-package-update~=23.7.1',
+   'ambient-package-update~=23.7.2',
    'gevent~=22.10',
 ]
 drf = [
    'djangorestframework>=3.8.2',
 ]
 graphql = [
    'graphene-django>=2.2.0',
@@ -134,15 +132,15 @@
 
 # Assume Python 3.11
 target-version = "py311"
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
-envlist = py{38,39,310,311}-django{22,30,31,32,40,41,42}
+envlist = py{38,39,310,311}-django{32,41,42}
 isolated_build = True
 
 [testenv]
 # Django deprecation overview: https://www.djangoproject.com/download/
 deps =
     django32: Django>=3.2,<3.3
     django41: Django>=4.1,<4.2
```

### Comparing `ambient_toolbox-8.4.3/settings.py` & `ambient_toolbox-9.0.0/settings.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/testapp/api/views.py` & `ambient_toolbox-9.0.0/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/testapp/migrations/0001_initial.py` & `ambient_toolbox-9.0.0/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/testapp/models.py` & `ambient_toolbox-9.0.0/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/testapp/templates/403.html` & `ambient_toolbox-9.0.0/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ambient_toolbox-9.0.0/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/ambient_toolbox/test_test_structure_validator.py` & `ambient_toolbox-9.0.0/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/drf/test_fields.py` & `ambient_toolbox-9.0.0/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/permissions/fixtures/test_declarations.py` & `ambient_toolbox-9.0.0/tests/permissions/fixtures/test_declarations.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/permissions/fixtures/test_helpers.py` & `ambient_toolbox-9.0.0/tests/permissions/fixtures/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/permissions/fixtures/test_services_setup_service.py` & `ambient_toolbox-9.0.0/tests/permissions/fixtures/test_services_setup_service.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/permissions/test_install_permission_fixtures_command.py` & `ambient_toolbox-9.0.0/tests/permissions/test_install_permission_fixtures_command.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/query_selectors/test_permission.py` & `ambient_toolbox-9.0.0/tests/query_selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/sentry/mock_data.py` & `ambient_toolbox-9.0.0/tests/sentry/mock_data.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/sentry/test_sentry_helper.py` & `ambient_toolbox-9.0.0/tests/sentry/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_admin_forms.py` & `ambient_toolbox-9.0.0/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_admin_inlines.py` & `ambient_toolbox-9.0.0/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_admin_model_admins_classes.py` & `ambient_toolbox-9.0.0/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_admin_view_mixins.py` & `ambient_toolbox-9.0.0/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_context_manager.py` & `ambient_toolbox-9.0.0/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_log_whodid.py` & `ambient_toolbox-9.0.0/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_managers.py` & `ambient_toolbox-9.0.0/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_math.py` & `ambient_toolbox-9.0.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_middleware.py` & `ambient_toolbox-9.0.0/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_mixins_models.py` & `ambient_toolbox-9.0.0/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_models.py` & `ambient_toolbox-9.0.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_rest_api_mixins.py` & `ambient_toolbox-9.0.0/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_scrubbing_service.py` & `ambient_toolbox-9.0.0/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_utils_date.py` & `ambient_toolbox-9.0.0/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_utils_file.py` & `ambient_toolbox-9.0.0/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_utils_model.py` & `ambient_toolbox-9.0.0/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_utils_named_tuple.py` & `ambient_toolbox-9.0.0/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/test_utils_string.py` & `ambient_toolbox-9.0.0/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/tests/mixins/test_django_message_framework.py` & `ambient_toolbox-9.0.0/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/tests/mixins/test_request_provider_mixin.py` & `ambient_toolbox-9.0.0/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/tests/test_mail_backends.py` & `ambient_toolbox-9.0.0/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/view_layer/test_formset_mixins.py` & `ambient_toolbox-9.0.0/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/view_layer/test_htmx_response_mixin.py` & `ambient_toolbox-9.0.0/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/view_layer/test_meta_mixins.py` & `ambient_toolbox-9.0.0/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/tests/view_layer/test_views.py` & `ambient_toolbox-9.0.0/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ambient_toolbox-8.4.3/PKG-INFO` & `ambient_toolbox-9.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 Metadata-Version: 2.1
 Name: ambient-toolbox
-Version: 8.4.3
+Version: 9.0.0
 Summary: Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
-Requires-Dist: Django>=2.2.28
+Requires-Dist: Django>=3.2.20
 Requires-Dist: bleach>=1.4,<6
 Requires-Dist: python-dateutil>=2.5.3
 Requires-Dist: freezegun~=1.2 ; extra == "dev"
 Requires-Dist: pytest-django~=4.5 ; extra == "dev"
 Requires-Dist: pytest-mock~=3.10 ; extra == "dev"
 Requires-Dist: pre-commit~=3.2 ; extra == "dev"
 Requires-Dist: black~=23.3 ; extra == "dev"
 Requires-Dist: Django~=3.2 ; extra == "dev"
 Requires-Dist: sphinx==4.2.0 ; extra == "dev"
 Requires-Dist: sphinx-rtd-theme==1.0.0 ; extra == "dev"
 Requires-Dist: m2r2==0.3.1 ; extra == "dev"
 Requires-Dist: mistune<2.0.0 ; extra == "dev"
-Requires-Dist: ambient-package-update~=23.7.1 ; extra == "dev"
+Requires-Dist: ambient-package-update~=23.7.2 ; extra == "dev"
 Requires-Dist: gevent~=22.10 ; extra == "dev"
 Requires-Dist: djangorestframework>=3.8.2 ; extra == "drf"
 Requires-Dist: graphene-django>=2.2.0 ; extra == "graphql"
 Requires-Dist: django-graphql-jwt>=0.2.1 ; extra == "graphql"
 Requires-Dist: sentry-sdk>=1.19.1 ; extra == "sentry"
 Requires-Dist: django-crispy-forms>=1.4.0 ; extra == "view-layer"
 Project-URL: Bugtracker, https://github.com/ambient-innovation/ambient-toolbox/issues
```

