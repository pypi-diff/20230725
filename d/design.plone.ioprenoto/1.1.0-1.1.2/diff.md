# Comparing `tmp/design.plone.ioprenoto-1.1.0.tar.gz` & `tmp/design.plone.ioprenoto-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.ioprenoto-1.1.0.tar", last modified: Fri Jun 30 06:48:24 2023, max compression
+gzip compressed data, was "design.plone.ioprenoto-1.1.2.tar", last modified: Tue Jul 25 08:34:22 2023, max compression
```

## Comparing `design.plone.ioprenoto-1.1.0.tar` & `design.plone.ioprenoto-1.1.2.tar`

### file list

```diff
@@ -1,111 +1,109 @@
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.918298 design.plone.ioprenoto-1.1.0/
--rw-r--r--   0 cekk       (501) staff       (20)     1414 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/CHANGES.rst
--rw-r--r--   0 cekk       (501) staff       (20)       58 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/CONTRIBUTORS.rst
--rw-r--r--   0 cekk       (501) staff       (20)     1338 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/DEVELOP.rst
--rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/LICENSE.GPL
--rw-r--r--   0 cekk       (501) staff       (20)      662 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/LICENSE.rst
--rw-r--r--   0 cekk       (501) staff       (20)      136 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/MANIFEST.in
--rw-r--r--   0 cekk       (501) staff       (20)     9034 2023-06-30 06:48:24.918498 design.plone.ioprenoto-1.1.0/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     4344 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/README.rst
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.900755 design.plone.ioprenoto-1.1.0/docs/
--rw-r--r--   0 cekk       (501) staff       (20)     7986 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/docs/conf.py
--rw-r--r--   0 cekk       (501) staff       (20)       89 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/docs/index.rst
--rw-r--r--   0 cekk       (501) staff       (20)      340 2023-06-30 06:48:24.919011 design.plone.ioprenoto-1.1.0/setup.cfg
--rw-r--r--   0 cekk       (501) staff       (20)     2774 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/setup.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.894194 design.plone.ioprenoto-1.1.0/src/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.900994 design.plone.ioprenoto-1.1.0/src/design/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.903342 design.plone.ioprenoto-1.1.0/src/design/plone/
--rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.904911 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/
--rw-r--r--   0 cekk       (501) staff       (20)      139 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.905626 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      562 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1471 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/stringinterp.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.906360 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1392 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/additional_fields.py
--rw-r--r--   0 cekk       (501) staff       (20)      591 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.906794 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      628 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.907113 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/overrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/overrides/.gitkeep
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.907305 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/static/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/static/.gitkeep
--rw-r--r--   0 cekk       (501) staff       (20)     1530 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.908067 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/
--rw-r--r--   0 cekk       (501) staff       (20)       24 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      481 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      136 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/events/on_create.py
--rw-r--r--   0 cekk       (501) staff       (20)      270 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/interfaces.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.909299 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/
--rw-r--r--   0 cekk       (501) staff       (20)      611 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/README.rst
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)     1520 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.895723 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.909810 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1395 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.896002 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.910367 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
--rw-r--r--   0 cekk       (501) staff       (20)      458 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.mo
--rw-r--r--   0 cekk       (501) staff       (20)     1395 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
--rw-r--r--   0 cekk       (501) staff       (20)     1754 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.py
--rwxr-xr-x   0 cekk       (501) staff       (20)      503 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.sh
--rw-r--r--   0 cekk       (501) staff       (20)      273 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/permissions.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.896662 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911354 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/
--rw-r--r--   0 cekk       (501) staff       (20)      191 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
--rw-r--r--   0 cekk       (501) staff       (20)      105 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/catalog.xml
--rw-r--r--   0 cekk       (501) staff       (20)      191 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/metadata.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911640 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/registry/
--rw-r--r--   0 cekk       (501) staff       (20)      180 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/registry/main.xml
--rw-r--r--   0 cekk       (501) staff       (20)      340 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/rolemap.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.911900 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/types/
--rw-r--r--   0 cekk       (501) staff       (20)      325 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.912143 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/uninstall/
--rw-r--r--   0 cekk       (501) staff       (20)      132 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.912659 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      280 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.913089 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      166 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.914059 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      414 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     1742 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
--rw-r--r--   0 cekk       (501) staff       (20)     2773 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.914306 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.915011 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/
--rw-r--r--   0 cekk       (501) staff       (20)      478 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)     6155 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.915730 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
--rw-r--r--   0 cekk       (501) staff       (20)      354 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      744 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/search.py
--rw-r--r--   0 cekk       (501) staff       (20)      201 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/configure.zcml
--rw-r--r--   0 cekk       (501) staff       (20)      794 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/setuphandlers.py
--rw-r--r--   0 cekk       (501) staff       (20)     2248 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/testing.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.917776 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/
--rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/__init__.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.918021 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/
--rw-r--r--   0 cekk       (501) staff       (20)     2019 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/test_example.robot
--rw-r--r--   0 cekk       (501) staff       (20)     1231 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
--rw-r--r--   0 cekk       (501) staff       (20)     2873 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
--rw-r--r--   0 cekk       (501) staff       (20)     3941 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
--rw-r--r--   0 cekk       (501) staff       (20)     2800 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
--rw-r--r--   0 cekk       (501) staff       (20)     7008 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
--rw-r--r--   0 cekk       (501) staff       (20)     2459 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_setup.py
--rw-r--r--   0 cekk       (501) staff       (20)     4844 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
-drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-30 06:48:24.903104 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/
--rw-r--r--   0 cekk       (501) staff       (20)     9034 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/PKG-INFO
--rw-r--r--   0 cekk       (501) staff       (20)     3964 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/SOURCES.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/dependency_links.txt
--rw-r--r--   0 cekk       (501) staff       (20)      147 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/entry_points.txt
--rw-r--r--   0 cekk       (501) staff       (20)       20 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
--rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/not-zip-safe
--rw-r--r--   0 cekk       (501) staff       (20)      293 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/requires.txt
--rw-r--r--   0 cekk       (501) staff       (20)        7 2023-06-30 06:48:24.000000 design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/top_level.txt
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.328532 design.plone.ioprenoto-1.1.2/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1627 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/CHANGES.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       58 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/CONTRIBUTORS.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1338 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/DEVELOP.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/LICENSE.GPL
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      662 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/LICENSE.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/MANIFEST.in
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7195 2023-07-25 08:34:22.328532 design.plone.ioprenoto-1.1.2/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4351 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/README.rst
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/docs/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7986 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/docs/conf.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       89 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/docs/index.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-07-25 08:34:22.328532 design.plone.ioprenoto-1.1.2/setup.cfg
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2774 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/setup.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/design/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      139 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      562 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1471 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/stringinterp.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1690 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/additional_fields.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      591 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      628 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/overrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/overrides/.gitkeep
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/static/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/static/.gitkeep
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1530 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/events/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       24 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/events/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      481 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/events/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      136 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/events/on_create.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      270 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/interfaces.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/README.rst
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1520 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/en/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/it/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1395 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1754 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/update.py
+-rwxrwxr-x   0 mauro     (1000) mauro     (1000)      503 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/update.sh
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/permissions.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/browserlayer.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      105 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/catalog.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      191 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/metadata.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/registry/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      180 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/registry/main.xml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      340 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/rolemap.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/types/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      325 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/uninstall/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      132 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/profiles/uninstall/browserlayer.xml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      280 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      166 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/configure.zcml
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      414 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1774 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2773 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookable_list/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      520 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookable_list/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     6698 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.324532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookings/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookings/__init__.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      354 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookings/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      813 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookings/search.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      201 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/configure.zcml
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      794 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/setuphandlers.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2248 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/testing.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.328532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/__init__.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.328532 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/robot/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2019 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/robot/test_example.robot
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     1231 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2873 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3962 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2800 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7501 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     2459 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_setup.py
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     4844 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py
+drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-07-25 08:34:22.320532 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     7195 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/PKG-INFO
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)     3812 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/SOURCES.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/dependency_links.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      127 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/entry_points.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/namespace_packages.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/not-zip-safe
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)      293 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/requires.txt
+-rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-07-25 08:34:22.000000 design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/top_level.txt
```

### Comparing `design.plone.ioprenoto-1.1.0/CHANGES.rst` & `design.plone.ioprenoto-1.1.2/CHANGES.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+1.1.2 (2023-07-25)
+------------------
+
+- Fix redireect url for anonymous
+  [mamico]
+
+- Changed label 'uffici correalti'
+  [mamico]
+
+1.1.1 (2023-07-07)
+------------------
+
+- fix booking_url in @bookings
+  [mamico]
 
 1.1.0 (2023-06-30)
 ------------------
 
 - Move message to contentrule in iocittadino
   [mamico]
```

### Comparing `design.plone.ioprenoto-1.1.0/DEVELOP.rst` & `design.plone.ioprenoto-1.1.2/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/LICENSE.GPL` & `design.plone.ioprenoto-1.1.2/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/LICENSE.rst` & `design.plone.ioprenoto-1.1.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/README.rst` & `design.plone.ioprenoto-1.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 - `referenced_by_prenotazioni_folder` which idicates if it has backreferences to PrenotazioniFolder 
   (design.plone.ioprenoto) throught correlated UO (with "Uffici correlati" field)
 
 PrenotazioniFolder serializer
 -----------------------------
 
-There is a customization of PrenotazioniFolder serializer that redirects to '/prenotazione-appuntamento'
+There is a customization of PrenotazioniFolder serializer that redirects to '/prenotazione-appuntamenti-uffici'
 if the user has not `design.plone.ioprenoto.ManagePrenotazioni`.
 
 @bookable-uo-list
 -----------------
 
 Endpoint that returns a list of *UnitaOrganizzativa* contents that have at least one PrenotazioniFolder that 
 relates to it (with "Uffici correlati" field).
```

### Comparing `design.plone.ioprenoto-1.1.0/docs/conf.py` & `design.plone.ioprenoto-1.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/setup.py` & `design.plone.ioprenoto-1.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.ioprenoto",
-    version="1.1.0",
+    version="1.1.2",
     description="An add-on for Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Plone",
         "Framework :: Plone :: Addon",
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/configure.zcml` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/adapters/stringinterp.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/adapters/stringinterp.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/additional_fields.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/additional_fields.py`

 * *Files 20% similar despite different names*

```diff
@@ -16,16 +16,21 @@
 
     orario_di_apertura = Text(
         title=_("Orario di apertura"),
         description=_("Orario di apertura della stanza prenotazioni"),
         required=False,
     )
     uffici_correlati = RelationList(
-        title=_("Uffici correlati"),
-        description=_("Uffici correlati al contesto corrente"),
+        title=_("Ufficio/i di riferimento"),
+        description=_(
+            "Uno o più uffici che utilizzano questa stanza per le prenotazioni online. "
+            "All'interno della scheda servizio è possibile specificare queste unità "
+            "organizzative, nel campo 'Canale fisico', o in assenza di questo, nel "
+            "campo 'Unità organizzativa responsabile'."
+        ),
         value_type=RelationChoice(
             title=_("Ufficio"),
             source=CatalogSource(portal_type="UnitaOrganizzativa"),
         ),
     )
 
     directives.widget(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/behaviors/configure.zcml` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/behaviors/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/browser/configure.zcml` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/configure.zcml` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/README.rst` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/locales/update.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/prenotazioniFolder.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from plone.restapi.serializer.summary import DefaultJSONSummarySerializer
 from redturtle.prenotazioni.content.prenotazioni_folder import IPrenotazioniFolder
 from zope.component import adapter
 from zope.interface import implementer
 
 
 PRENOTAZIONI_MANAGE_PERMISSION = "redturtle.prenotazioni: Manage Prenotazioni"
-PRENOTAZIONE_APPUNTAMENTO_ADDRESS = "prenotazione-appuntamento"
+# TODO: move to registry
+PRENOTAZIONE_APPUNTAMENTO_ADDRESS = "prenotazione-appuntamenti-uffici"
 
 
 @implementer(ISerializeToJsonSummary)
 @adapter(IPrenotazioniFolder, IDesignPloneIoprenotoLayer)
 class SerializePrenotazioniFolderToJsonSummary(DefaultJSONSummarySerializer):
     def __call__(self, *args, **kwargs):
         if not api.user.has_permission(
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/serializers/ovverrides/servizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookable_list/get.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # -*- coding: utf-8 -*-
+from urllib.parse import urlencode
+
 from plone import api
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.services import Service
-from urllib.parse import urlencode
 from zc.relation.interfaces import ICatalog
-from zope.component import getMultiAdapter
-from zope.component import getUtility
+from zope.component import getMultiAdapter, getUtility
 from zope.intid.interfaces import IIntIds
+from plone.restapi.serializer.converters import json_compatible
 
 
 class BookableList(Service):
     def reply(self):
         """
         Return all UO with at least one back-refence from PrenotazioniFolder
         """
@@ -56,14 +57,18 @@
                                     "url": f"{portal_url}/prenotazione-appuntamenti-uffici?{query}",  # noqa: E501
                                     "booking_type": booking_type["name"],
                                     "booking_duration": booking_type.get("duration"),
                                     "service_title": brain_service.Title,
                                     "booking_opening_hours": prenotazioni_folder.orario_di_apertura,  # noqa: E501
                                     "address": sede,
                                     "uo_title": brain_uo.Title,
+                                    "description_agenda": json_compatible(
+                                        prenotazioni_folder.descriptionAgenda,
+                                        prenotazioni_folder,
+                                    ),  # noqa: E501
                                 }
                             )
         return response
 
     def get_sede(self, uo):
         ref = getattr(uo, "sede", [])
         if not ref:
@@ -130,14 +135,18 @@
                     folders.append(
                         {
                             "@id": prenotazioni_folder.absolute_url(),
                             "uid": prenotazioni_folder.UID(),
                             "title": prenotazioni_folder.Title(),
                             "orario_di_apertura": prenotazioni_folder.orario_di_apertura,
                             "address": sede,
+                            "description_agenda": json_compatible(
+                                prenotazioni_folder.descriptionAgenda,
+                                prenotazioni_folder,
+                            ),  # noqa: E501
                         }
                     )
             if folders:
                 response["items"].append(
                     {
                         "@id": uo.absolute_url(),
                         "title": uo.Title(),
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/restapi/services/bookings/search.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/restapi/services/bookings/search.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
+from plone import api
 from redturtle.prenotazioni.restapi.services.bookings.search import (
     BookingsSearch as BookingsSearchBase,
 )  # noqa: E501
 from zope.interface import implementer
 from zope.publisher.interfaces import IPublishTraverse
-from plone import api
 
 
+# TODO: in alternativa si poteva sovrascrivere il serializer
 @implementer(IPublishTraverse)
 class BookingsSearch(BookingsSearchBase):
     def reply(self):
         response = super(BookingsSearch, self).reply()
         base_url = api.portal.get_registry_record(
             name="volto.frontend_domain", default=""
         )
         base_url = f"{base_url}/prenotazione-appuntamenti-uffici"
         for item in response.get("items") or []:
-            item["url"] = f"{base_url}?booking_id={item['booking_id']}"
+            item["booking_url"] = f"{base_url}?booking_id={item['booking_id']}"
         return response
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/setuphandlers.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/testing.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/robot/test_example.robot` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/robot/test_example.robot`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_PrenotazioniFolder_ct.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_prenotazioni_messages.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_prenotazioni_folder.py`

 * *Files 7% similar despite different names*

```diff
@@ -64,27 +64,27 @@
         self.api_session_admin.close()
         self.api_session_user.close()
         self.api_session_editor.close()
         self.api_session_anon.close()
 
     def test_anon_redirected(self):
         self.assertIn(
-            "prenotazione-appuntamento",
+            "prenotazione-appuntamenti-uffici",
             self.api_session_anon.get(self.prenotazioni_folder.absolute_url()).url,
         )
 
     def test_user_redirected(self):
         self.assertIn(
-            "prenotazione-appuntamento",
+            "prenotazione-appuntamenti-uffici",
             self.api_session_user.get(self.prenotazioni_folder.absolute_url()).url,
         )
 
     def test_editor_redirected_where_cant_edit(self):
         self.assertIn(
-            "prenotazione-appuntamento",
+            "prenotazione-appuntamenti-uffici",
             self.api_session_editor.get(self.prenotazioni_folder2.absolute_url()).url,
         )
 
     def test_editor_can_access_if_have_permission(self):
         self.assertEquals(
             self.api_session_editor.get(self.prenotazioni_folder.absolute_url()).json()[
                 "@id"
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_serializers_ovverrides_serzvizio.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_restapi_service_bookable_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,22 @@
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from plone.restapi.testing import RelativeSession
 from transaction import commit
 from z3c.relationfield.relation import RelationValue
 from zope.component import getMultiAdapter
 from zope.component import queryUtility
 from zope.intid.interfaces import IIntIds
+from plone.app.textfield.value import RichTextValue
 
 import unittest
 
 
 class BookableUOListTest(unittest.TestCase):
     layer = DESIGN_PLONE_IOPRENOTO_API_FUNCTIONAL_TESTING
+    maxDiff = None
 
     def setUp(self):
         self.app = self.layer["app"]
         self.portal = self.layer["portal"]
         self.request = self.layer["request"]
         self.portal_url = self.portal.absolute_url()
 
@@ -57,14 +59,19 @@
         )
 
         self.prenotazioni_folder = api.content.create(
             container=self.portal,
             type="PrenotazioniFolder",
             title="Prenotazioni Folder",
             orario_di_apertura="foo",
+            descriptionAgenda=RichTextValue(
+                "<h1>description agenda</h1>",
+                "text/html",
+                "text/html",
+            ),
             uffici_correlati=[
                 RelationValue(
                     to_id=queryUtility(IIntIds).getId(self.unita_organizzativa)
                 )
             ],
             booking_types=[
                 {"name": "Type A", "duration": "30"},
@@ -160,14 +167,22 @@
             prenotazioni_folder["orario_di_apertura"],
             self.prenotazioni_folder.orario_di_apertura,
         )
         self.assertEqual(
             prenotazioni_folder["address"],
             getMultiAdapter((self.venue, self.request), ISerializeToJsonSummary)(),
         )
+        self.assertEqual(
+            prenotazioni_folder["description_agenda"],
+            {
+                "content-type": "text/html",
+                "data": "<h1>description agenda</h1>",
+                "encoding": "utf-8",
+            },
+        )
 
     def test_endpoint_return_filtered_uo_based_on_service_uid(self):
         resp = self.api_session.get(
             f"{self.portal_url}/@bookable-uo-list?uid=foo"
         ).json()
         self.assertEqual(resp["items"], [])
```

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_setup.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py` & `design.plone.ioprenoto-1.1.2/src/design/plone/ioprenoto/tests/test_stringinterp_overrides.py`

 * *Files identical despite different names*

### Comparing `design.plone.ioprenoto-1.1.0/src/design.plone.ioprenoto.egg-info/SOURCES.txt` & `design.plone.ioprenoto-1.1.2/src/design.plone.ioprenoto.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 src/design/plone/ioprenoto/events/configure.zcml
 src/design/plone/ioprenoto/events/on_create.py
 src/design/plone/ioprenoto/locales/README.rst
 src/design/plone/ioprenoto/locales/__init__.py
 src/design/plone/ioprenoto/locales/design.plone.ioprenoto.pot
 src/design/plone/ioprenoto/locales/update.py
 src/design/plone/ioprenoto/locales/update.sh
-src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.mo
 src/design/plone/ioprenoto/locales/en/LC_MESSAGES/design.plone.ioprenoto.po
-src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.mo
 src/design/plone/ioprenoto/locales/it/LC_MESSAGES/design.plone.ioprenoto.po
 src/design/plone/ioprenoto/profiles/default/browserlayer.xml
 src/design/plone/ioprenoto/profiles/default/catalog.xml
 src/design/plone/ioprenoto/profiles/default/metadata.xml
 src/design/plone/ioprenoto/profiles/default/rolemap.xml
 src/design/plone/ioprenoto/profiles/default/registry/main.xml
 src/design/plone/ioprenoto/profiles/default/types/PrenotazioniFolder.xml
```

