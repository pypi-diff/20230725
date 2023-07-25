# Comparing `tmp/skip-django-pymess-0.7.6.2.tar.gz` & `tmp/skip-django-pymess-0.7.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skip-django-pymess-0.7.6.2.tar", last modified: Thu Jul 20 13:15:49 2023, max compression
+gzip compressed data, was "skip-django-pymess-0.7.6.3.tar", last modified: Tue Jul 25 21:07:37 2023, max compression
```

## Comparing `skip-django-pymess-0.7.6.2.tar` & `skip-django-pymess-0.7.6.3.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/
--rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/controlers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/dialer/
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/daktela.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/dialer/dummy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/emails/
--rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/emails/smtp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.345599 skip-django-pymess-0.7.6.2/pymess/backend/push/
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/push/onesignal.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/routers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/backend/sms/
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/ats_sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/sms_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/backend/sms/twilio.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/enums.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.349599 skip-django-pymess-0.7.6.2/pymess/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/check_dialer_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/check_sms_delivery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/dump_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/pull_emails_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/send_messages_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/management/commands/sync_emails.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.353599 skip-django-pymess-0.7.6.2/pymess/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0003_dialer.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0004_dialermessage_is_final_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0005_push_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0006_auto_20190322_1712.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0007_auto_20190401_1145.py
--rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0008_auto_20190726_1459.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0009_20191108_2007.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0010_20191120_1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0011_auto_20191210_1749.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0012_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0013_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0014_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0015_auto_20200110_0904.py
--rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0016_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0017_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0018_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0019_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0020_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0021_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0022_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0023_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0024_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0025_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0026_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0027_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/0028_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/models/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/dialer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/emails.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/push.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/models/sms.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/pymess/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.341599 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/base.xml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/ats/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/base.xml
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templates/pymess/sms/sms_operator/sms.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/templatetags/pymess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/html.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/logged_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/utils/migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/pymess/webhooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/pymess/webhooks/mandrill.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 13:15:49.361600 skip-django-pymess-0.7.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 13:15:39.000000 skip-django-pymess-0.7.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 13:15:49.357600 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-20 13:15:49.000000 skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.404618 skip-django-pymess-0.7.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 21:07:37.404618 skip-django-pymess-0.7.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.388617 skip-django-pymess-0.7.6.3/pymess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.388617 skip-django-pymess-0.7.6.3/pymess/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)    11865 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/controlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.388617 skip-django-pymess-0.7.6.3/pymess/backend/dialer/
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/dialer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/dialer/daktela.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/dialer/dummy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.388617 skip-django-pymess-0.7.6.3/pymess/backend/emails/
+-rw-r--r--   0 runner    (1001) docker     (123)     6279 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/emails/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/emails/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/emails/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/emails/smtp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.388617 skip-django-pymess-0.7.6.3/pymess/backend/push/
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/push/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/push/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/push/onesignal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/routers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.392617 skip-django-pymess-0.7.6.3/pymess/backend/sms/
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/ats_sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9661 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/sms_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/backend/sms/twilio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/enums.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.384616 skip-django-pymess-0.7.6.3/pymess/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.384616 skip-django-pymess-0.7.6.3/pymess/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.392617 skip-django-pymess-0.7.6.3/pymess/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     9614 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    14115 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.392617 skip-django-pymess-0.7.6.3/pymess/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.392617 skip-django-pymess-0.7.6.3/pymess/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/check_dialer_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/check_sms_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/dump_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/pull_emails_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/send_messages_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/management/commands/sync_emails.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0002_emailmessage_number_of_send_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0003_dialer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0004_dialermessage_is_final_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0005_push_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0006_auto_20190322_1712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0007_auto_20190401_1145.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0008_auto_20190726_1459.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0009_20191108_2007.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0010_20191120_1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0011_auto_20191210_1749.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0012_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0013_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0014_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0015_auto_20200110_0904.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6038 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0016_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0017_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0018_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0019_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0020_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0021_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0022_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0023_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0024_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0025_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0026_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0027_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/0028_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9842 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/dialer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10611 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/push.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/models/sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.384616 skip-django-pymess-0.7.6.3/pymess/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.384616 skip-django-pymess-0.7.6.3/pymess/templates/pymess/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.384616 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/ats/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/ats/base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/ats/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/ats/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/sms_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/sms_operator/base.xml
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/sms_operator/delivery_request.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templates/pymess/sms/sms_operator/sms.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/templatetags/pymess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.400618 skip-django-pymess-0.7.6.3/pymess/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/utils/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/utils/logged_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1349 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/utils/migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.404618 skip-django-pymess-0.7.6.3/pymess/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/pymess/webhooks/mandrill.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-25 21:07:37.404618 skip-django-pymess-0.7.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-25 21:07:25.000000 skip-django-pymess-0.7.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 21:07:37.404618 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-25 21:07:37.000000 skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/top_level.txt
```

### Comparing `skip-django-pymess-0.7.6.2/LICENSE` & `skip-django-pymess-0.7.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/PKG-INFO` & `skip-django-pymess-0.7.6.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.6.2
+Version: 0.7.6.3
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/dialer/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/backend/dialer/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/dialer/daktela.py` & `skip-django-pymess-0.7.6.3/pymess/backend/dialer/daktela.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/emails/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/backend/emails/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/emails/dummy.py` & `skip-django-pymess-0.7.6.3/pymess/backend/emails/dummy.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/emails/mandrill.py` & `skip-django-pymess-0.7.6.3/pymess/backend/emails/mandrill.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/emails/smtp.py` & `skip-django-pymess-0.7.6.3/pymess/backend/emails/smtp.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/push/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/backend/push/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/push/onesignal.py` & `skip-django-pymess-0.7.6.3/pymess/backend/push/onesignal.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/sms/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/backend/sms/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/sms/ats_sms_operator.py` & `skip-django-pymess-0.7.6.3/pymess/backend/sms/ats_sms_operator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/sms/sms_operator.py` & `skip-django-pymess-0.7.6.3/pymess/backend/sms/sms_operator.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/sms/sns.py` & `skip-django-pymess-0.7.6.3/pymess/backend/sms/sns.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/backend/sms/twilio.py` & `skip-django-pymess-0.7.6.3/pymess/backend/sms/twilio.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/config.py` & `skip-django-pymess-0.7.6.3/pymess/config.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/enums.py` & `skip-django-pymess-0.7.6.3/pymess/enums.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.mo` & `skip-django-pymess-0.7.6.3/pymess/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/locale/cs/LC_MESSAGES/django.po` & `skip-django-pymess-0.7.6.3/pymess/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/management/commands/dump_emails.py` & `skip-django-pymess-0.7.6.3/pymess/management/commands/dump_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/management/commands/pull_emails_info.py` & `skip-django-pymess-0.7.6.3/pymess/management/commands/pull_emails_info.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/management/commands/send_messages_batch.py` & `skip-django-pymess-0.7.6.3/pymess/management/commands/send_messages_batch.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/management/commands/sync_emails.py` & `skip-django-pymess-0.7.6.3/pymess/management/commands/sync_emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0001_initial.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0003_dialer.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0003_dialer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0005_push_notifications.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0005_push_notifications.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0006_auto_20190322_1712.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0006_auto_20190322_1712.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0007_auto_20190401_1145.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0007_auto_20190401_1145.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0008_auto_20190726_1459.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0008_auto_20190726_1459.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0009_20191108_2007.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0009_20191108_2007.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0010_20191120_1002.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0010_20191120_1002.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0011_auto_20191210_1749.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0011_auto_20191210_1749.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0012_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0012_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0013_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0013_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0014_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0014_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0015_auto_20200110_0904.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0015_auto_20200110_0904.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0016_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0016_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0017_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0017_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0018_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0018_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0019_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0019_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0020_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0020_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0021_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0021_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0022_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0022_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0023_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0023_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0024_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0024_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0025_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0025_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0026_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0026_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/migrations/0027_migration.py` & `skip-django-pymess-0.7.6.3/pymess/migrations/0027_migration.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/models/common.py` & `skip-django-pymess-0.7.6.3/pymess/models/common.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/models/dialer.py` & `skip-django-pymess-0.7.6.3/pymess/models/dialer.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/models/emails.py` & `skip-django-pymess-0.7.6.3/pymess/models/emails.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/models/push.py` & `skip-django-pymess-0.7.6.3/pymess/models/push.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/models/sms.py` & `skip-django-pymess-0.7.6.3/pymess/models/sms.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     class Meta(BaseRelatedObject.Meta):
         verbose_name = _('related object of a SMS message')
         verbose_name_plural = _('related objects of SMS messages')
 
 
 class AbstractSMSTemplate(BaseAbstractTemplate):
 
-    is_secret = models.BooleanField(null=False, blank=False, verbose_name=_('is secret'))
+    is_secret = models.BooleanField(null=False, blank=False, default=True, verbose_name=_('is secret'))
 
     def get_controller(self):
         from pymess.backend.sms import SMSController
         return SMSController()
 
     class Meta(BaseAbstractTemplate.Meta):
         abstract = True
```

### Comparing `skip-django-pymess-0.7.6.2/pymess/templatetags/pymess.py` & `skip-django-pymess-0.7.6.3/pymess/templatetags/pymess.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/utils/__init__.py` & `skip-django-pymess-0.7.6.3/pymess/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/utils/html.py` & `skip-django-pymess-0.7.6.3/pymess/utils/html.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/utils/logged_requests.py` & `skip-django-pymess-0.7.6.3/pymess/utils/logged_requests.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/utils/migrations.py` & `skip-django-pymess-0.7.6.3/pymess/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/pymess/webhooks/mandrill.py` & `skip-django-pymess-0.7.6.3/pymess/webhooks/mandrill.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/setup.py` & `skip-django-pymess-0.7.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/PKG-INFO` & `skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skip-django-pymess
-Version: 0.7.6.2
+Version: 0.7.6.3
 Summary: Pymess is a Django framework for sending messages
 Home-page: https://github.com/skip-pay/django-pymess
 Author: Lubos Matl,Oskar Hollman
 Author-email: matllubos@gmail.com
 License: LGPL
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Django
```

### Comparing `skip-django-pymess-0.7.6.2/skip_django_pymess.egg-info/SOURCES.txt` & `skip-django-pymess-0.7.6.3/skip_django_pymess.egg-info/SOURCES.txt`

 * *Files identical despite different names*

