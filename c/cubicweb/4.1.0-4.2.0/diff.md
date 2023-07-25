# Comparing `tmp/cubicweb-4.1.0.tar.gz` & `tmp/cubicweb-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-4.1.0.tar", last modified: Wed Jul  5 08:55:37 2023, max compression
+gzip compressed data, was "cubicweb-4.2.0.tar", last modified: Tue Jul 25 16:24:12 2023, max compression
```

## Comparing `cubicweb-4.1.0.tar` & `cubicweb-4.2.0.tar`

### file list

```diff
@@ -1,1322 +1,1324 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.257017 cubicweb-4.1.0/
--rw-rw-rw-   0 root         (0) root         (0)    17987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/COPYING
--rw-rw-rw-   0 root         (0) root         (0)    26527 2023-07-05 08:55:06.000000 cubicweb-4.1.0/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)     4926 2023-07-05 08:55:06.000000 cubicweb-4.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     4231 2023-07-05 08:55:37.257017 cubicweb-4.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.701010 cubicweb-4.1.0/cubicweb/
--rw-rw-rw-   0 root         (0) root         (0)     7348 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       69 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     6885 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/_gcdebug.py
--rw-rw-rw-   0 root         (0) root         (0)     5211 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/appobject.py
--rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    64892 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    32469 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)     4899 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwgettext.py
--rw-rw-rw-   0 root         (0) root         (0)    25984 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/cwvreg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.709010 cubicweb-4.1.0/cubicweb/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3276 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/csv.py
--rw-rw-rw-   0 root         (0) root         (0)    21024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/importer.py
--rw-rw-rw-   0 root         (0) root         (0)    26724 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)    15511 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)    18099 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/stores.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.713010 cubicweb-4.1.0/cubicweb/dataimport/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.717010 cubicweb-4.1.0/cubicweb/dataimport/test/data/
--rw-rw-rw-   0 root         (0) root         (0)   474710 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/geonames.csv
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/people.csv
--rw-rw-rw-   0 root         (0) root         (0)     1231 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data/timeZones.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.717010 cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/
--rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2513 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_csv.py
--rw-rw-rw-   0 root         (0) root         (0)    16178 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_massive_store.py
--rw-rw-rw-   0 root         (0) root         (0)     4179 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_pgstore.py
--rw-rw-rw-   0 root         (0) root         (0)     8221 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/test_stores.py
--rw-rw-rw-   0 root         (0) root         (0)    10720 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/dataimport/test/unittest_importer.py
--rw-rw-rw-   0 root         (0) root         (0)     2677 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.725010 cubicweb-4.1.0/cubicweb/devtools/
--rw-rw-rw-   0 root         (0) root         (0)    27150 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4116 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/apptest_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.725010 cubicweb-4.1.0/cubicweb/devtools/data/
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/cwmock.js
--rw-rw-rw-   0 root         (0) root         (0)     5146 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/qunit.css
--rw-rw-rw-   0 root         (0) root         (0)   115758 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/data/qunit.js
--rw-rw-rw-   0 root         (0) root         (0)    38090 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     3702 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fake.py
--rw-rw-rw-   0 root         (0) root         (0)    24604 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fill.py
--rwxrwxrwx   0 root         (0) root         (0)     1011 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/fix_po_encoding
--rw-rw-rw-   0 root         (0) root         (0)    10988 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/htmlparser.py
--rw-rw-rw-   0 root         (0) root         (0)     5298 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/httptest.py
--rw-rw-rw-   0 root         (0) root         (0)     9217 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     2354 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/realdbtest.py
--rw-rw-rw-   0 root         (0) root         (0)    10915 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/repotest.py
--rw-rw-rw-   0 root         (0) root         (0)     6775 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/stresstester.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.729010 cubicweb-4.1.0/cubicweb/devtools/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.729010 cubicweb-4.1.0/cubicweb/devtools/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)    11311 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/firstnames.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.605008 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.733010 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
--rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1679 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.605008 cubicweb-4.1.0/cubicweb/devtools/test/data/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.737010 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
--rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
--rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
--rw-rw-rw-   0 root         (0) root         (0)      321 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
--rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_dbfill.py
--rw-rw-rw-   0 root         (0) root         (0)     6325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_devctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2475 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_fill.py
--rw-rw-rw-   0 root         (0) root         (0)     3225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/test/unittest_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)    22045 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/devtools/testlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.741010 cubicweb-4.1.0/cubicweb/entities/
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24573 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/adapters.py
--rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/authobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4207 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     6010 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/schemaobjs.py
--rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/sources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.741010 cubicweb-4.1.0/cubicweb/entities/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/entities/test/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/entities/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9992 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/unittest_base.py
--rw-rw-rw-   0 root         (0) root         (0)    36515 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/test/unittest_wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    23208 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entities/wfobjs.py
--rw-rw-rw-   0 root         (0) root         (0)    59296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/ext/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5931 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/html4zope.py
--rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.745010 cubicweb-4.1.0/cubicweb/ext/test/
--rw-rw-rw-   0 root         (0) root         (0)     2013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/ext/test/unittest_markdown.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.753010 cubicweb-4.1.0/cubicweb/hooks/
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/email.py
--rw-rw-rw-   0 root         (0) root         (0)    13223 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     5680 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/metadata.py
--rw-rw-rw-   0 root         (0) root         (0)     9739 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/security.py
--rw-rw-rw-   0 root         (0) root         (0)    10642 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    60957 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4913 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2952 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/syncsources.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.757010 cubicweb-4.1.0/cubicweb/hooks/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/hooks/test/data/
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2728 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/hooks/test/data-computed/
--rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/data-computed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1729 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_bookmarks.py
--rw-rw-rw-   0 root         (0) root         (0)    13100 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     8490 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_integrity.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_notificationhooks.py
--rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_security.py
--rw-rw-rw-   0 root         (0) root         (0)     6277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_synccomputed.py
--rw-rw-rw-   0 root         (0) root         (0)    24444 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncschema.py
--rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsession.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsources.py
--rw-rw-rw-   0 root         (0) root         (0)    15886 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/hooks/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.761011 cubicweb-4.1.0/cubicweb/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    93082 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)    61668 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)   112148 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)   106920 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     3759 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/mail.py
--rw-rw-rw-   0 root         (0) root         (0)     3352 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/md5crypt.py
--rw-rw-rw-   0 root         (0) root         (0)    22103 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/migration.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.765010 cubicweb-4.1.0/cubicweb/misc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.769011 cubicweb-4.1.0/cubicweb/misc/migration/
--rw-rw-rw-   0 root         (0) root         (0)      690 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.1_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.22.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.23.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.24.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.24.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.27.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.30.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.31.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.32.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/3.38.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)    20222 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3370 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/migration/postcreate.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.773011 cubicweb-4.1.0/cubicweb/misc/scripts/
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/chpasswd.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/detect_cycle.py
--rw-rw-rw-   0 root         (0) root         (0)     5750 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/ldap_change_base_dn.py
--rw-rw-rw-   0 root         (0) root         (0)     3474 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/scripts/migration_helper.py
--rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/misc/source_highlight.py
--rw-rw-rw-   0 root         (0) root         (0)     3270 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/mttransforms.py
--rw-rw-rw-   0 root         (0) root         (0)    17407 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/multipart.py
--rw-rw-rw-   0 root         (0) root         (0)    50971 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/predicates.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.781011 cubicweb-4.1.0/cubicweb/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     9374 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     4572 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/config.py
--rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/core.py
--rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/csrf.py
--rw-rw-rw-   0 root         (0) root         (0)     7081 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_source_code.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.785011 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/
--rw-rw-rw-   0 root         (0) root         (0)     1895 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1505 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
--rw-rw-rw-   0 root         (0) root         (0)     3912 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     1592 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     4852 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     2980 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
--rw-rw-rw-   0 root         (0) root         (0)     8486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/debugtoolbar_panels.py
--rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/development.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     3771 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1632 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/pyramid.ini.tmpl
--rw-rw-rw-   0 root         (0) root         (0)    13542 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/pyramidctl.py
--rw-rw-rw-   0 root         (0) root         (0)     5310 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/resources.py
--rw-rw-rw-   0 root         (0) root         (0)     6854 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/rest_api.py
--rw-rw-rw-   0 root         (0) root         (0)     9634 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/
--rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/data/
--rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.789011 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_config.py
--rw-rw-rw-   0 root         (0) root         (0)     6519 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_content_negociation.py
--rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_core.py
--rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/test/test_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pyramid/tools.py
--rw-rw-rw-   0 root         (0) root         (0)     1929 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/pytestconf.py
--rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)     2170 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)    17499 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/req.py
--rw-rw-rw-   0 root         (0) root         (0)    41745 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    11506 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    27303 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rset.py
--rw-rw-rw-   0 root         (0) root         (0)    11717 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    57984 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     6147 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schema_exporters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.793011 cubicweb-4.1.0/cubicweb/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/Bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     1696 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1662 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/_regproc.postgres.sql
--rw-rw-rw-   0 root         (0) root         (0)    13898 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/base.py
--rw-rw-rw-   0 root         (0) root         (0)    15024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/bootstrap.py
--rw-rw-rw-   0 root         (0) root         (0)    11853 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/schemas/workflow.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.805011 cubicweb-4.1.0/cubicweb/server/
--rw-rw-rw-   0 root         (0) root         (0)    14123 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3275 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/check_unused_index.py
--rw-rw-rw-   0 root         (0) root         (0)    23459 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/checkintegrity.py
--rw-rw-rw-   0 root         (0) root         (0)     6110 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/edition.py
--rw-rw-rw-   0 root         (0) root         (0)    38611 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/hook.py
--rw-rw-rw-   0 root         (0) root         (0)    78083 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/migractions.py
--rw-rw-rw-   0 root         (0) root         (0)    35946 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/querier.py
--rw-rw-rw-   0 root         (0) root         (0)    47968 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/repository.py
--rw-rw-rw-   0 root         (0) root         (0)    19170 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    13967 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28738 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)     3168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/serverconfig.py
--rw-rw-rw-   0 root         (0) root         (0)    52134 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)    32452 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/session.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.809011 cubicweb-4.1.0/cubicweb/server/sources/
--rw-rw-rw-   0 root         (0) root         (0)    13281 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18201 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)    16790 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/ldapfeed.py
--rw-rw-rw-   0 root         (0) root         (0)    78435 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/native.py
--rw-rw-rw-   0 root         (0) root         (0)    71413 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    11169 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sources/storages.py
--rw-rw-rw-   0 root         (0) root         (0)    22724 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)    22491 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/ssplanner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.821011 cubicweb-4.1.0/cubicweb/server/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.825011 cubicweb-4.1.0/cubicweb/server/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.861012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.865012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.865012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/ldap_test.ldif
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/slapd.conf.in
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/sources_extern
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data/sources_multi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.825011 cubicweb-4.1.0/cubicweb/server/test/data-cwep002/
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-cwep002/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.829011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.829011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.833011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.837011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.837011 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.841012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.841012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.845012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.849012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.849012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.853012 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.857012 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/
--rw-rw-rw-   0 root         (0) root         (0)     2510 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Company.py
--rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
--rw-rw-rw-   0 root         (0) root         (0)     3298 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/State.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3778 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/toignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.857012 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8829 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_datafeed.py
--rw-rw-rw-   0 root         (0) root         (0)     2192 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_edition.py
--rw-rw-rw-   0 root         (0) root         (0)     4881 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_hook.py
--rw-rw-rw-   0 root         (0) root         (0)    24766 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_ldapsource.py
--rw-rw-rw-   0 root         (0) root         (0)    96667 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_querier.py
--rw-rw-rw-   0 root         (0) root         (0)   101035 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_rql2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    23311 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_rqlannotation.py
--rw-rw-rw-   0 root         (0) root         (0)    11087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_schema2sql.py
--rw-rw-rw-   0 root         (0) root         (0)    28099 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_schemaserial.py
--rw-rw-rw-   0 root         (0) root         (0)    38100 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_server_security.py
--rw-rw-rw-   0 root         (0) root         (0)     5431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_server_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_serverctl.py
--rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_sources_native.py
--rw-rw-rw-   0 root         (0) root         (0)     2449 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_sqlutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_ssplanner.py
--rw-rw-rw-   0 root         (0) root         (0)    17471 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_storage.py
--rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_tools.py
--rw-rw-rw-   0 root         (0) root         (0)    21794 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_undo.py
--rw-rw-rw-   0 root         (0) root         (0)     2619 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test/unittest_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.869012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.873012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.873012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.877012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.877012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.881012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_migractions/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.885012 cubicweb-4.1.0/cubicweb/server/test_migractions/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.917013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.889012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.889012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.893012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.897012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.897012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.901012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.905012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.905012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.909012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.909012 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.913013 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.921013 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)    47736 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.925013 cubicweb-4.1.0/cubicweb/server/test_migractions2/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.925013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.957013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.961013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.929013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.929013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.933013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.933013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.937013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.937013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.941013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.945013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.945013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.949013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.953013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.953013 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9732 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions2/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.965013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.993013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.997014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/
--rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.969013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.973013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.973013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.977013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.981013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.981013 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.985014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.989014 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1972 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_migractions3/unittest_migractions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.001014 cubicweb-4.1.0/cubicweb/server/test_postgres/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.005014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.005014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.009014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/postcreate.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/data/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    10234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_postgres/unittest_postgres.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.013014 cubicweb-4.1.0/cubicweb/server/test_repository/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.021014 cubicweb-4.1.0/cubicweb/server/test_repository/data/
--rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.025014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.029014 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.021014 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/
--rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
--rw-rw-rw-   0 root         (0) root         (0)    37991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/test_repository/unittest_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/server/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.033014 cubicweb-4.1.0/cubicweb/skeleton/
--rw-rw-rw-   0 root         (0) root         (0)     1112 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.hgignore.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/.yamllint.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/Dockerfile.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/MANIFEST.in.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1484 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/README.rst.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.037014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/
--rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
--rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
--rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/setup.py.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.041014 cubicweb-4.1.0/cubicweb/skeleton/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.045014 cubicweb-4.1.0/cubicweb/skeleton/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
--rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/skeleton/tox.ini.tmpl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.045014 cubicweb-4.1.0/cubicweb/smoke_test/
--rw-rw-rw-   0 root         (0) root         (0)     1433 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1364 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12952 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/ldapparser.py
--rw-rw-rw-   0 root         (0) root         (0)    14620 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5869 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/services.py
--rw-rw-rw-   0 root         (0) root         (0)     8236 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/supervising.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.049014 cubicweb-4.1.0/cubicweb/sobjects/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.053014 cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/
--rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4020 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_email.py
--rw-rw-rw-   0 root         (0) root         (0)     3061 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_notification.py
--rw-rw-rw-   0 root         (0) root         (0)     5404 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_register_user.py
--rw-rw-rw-   0 root         (0) root         (0)     5051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/sobjects/test/unittest_supervising.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/tags.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.065014 cubicweb-4.1.0/cubicweb/test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.069015 cubicweb-4.1.0/cubicweb/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.077015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.077015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/entities.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/hooks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/views/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/views/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/entities/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.081015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/hooks/
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.085015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/
--rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.089015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/
--rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.089015 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/erqlexpr_on_ertype.py
--rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/lowered_etype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.093015 cubicweb-4.1.0/cubicweb/test/data/migration/
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.0.3_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.0.4_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_common.py
--rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/migration/0.1.2_Any.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_computedrel.py
--rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
--rw-rw-rw-   0 root         (0) root         (0)     1401 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_attr.py
--rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_eetype.py
--rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.093015 cubicweb-4.1.0/cubicweb/test/data/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script1.py
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script2.py
--rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/scripts/script3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.097015 cubicweb-4.1.0/cubicweb/test/data/server_migration/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data/uppered_rtype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.069015 cubicweb-4.1.0/cubicweb/test/data-rewrite/
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.073015 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.073015 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data-rewrite/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.097015 cubicweb-4.1.0/cubicweb/test/data_schemareader/
--rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/data_schemareader/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_binary.py
--rw-rw-rw-   0 root         (0) root         (0)      404 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_crypto.py
--rw-rw-rw-   0 root         (0) root         (0)    17528 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_cwconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     7427 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_cwctl.py
--rw-rw-rw-   0 root         (0) root         (0)    48020 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_entity.py
--rw-rw-rw-   0 root         (0) root         (0)     4855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_fast_drop_entities.py
--rw-rw-rw-   0 root         (0) root         (0)     8359 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_mail.py
--rw-rw-rw-   0 root         (0) root         (0)     7471 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_migration.py
--rw-rw-rw-   0 root         (0) root         (0)    15441 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_repoapi.py
--rw-rw-rw-   0 root         (0) root         (0)     5855 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_req.py
--rw-rw-rw-   0 root         (0) root         (0)    45868 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rqlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6509 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rqlsuggestions.py
--rw-rw-rw-   0 root         (0) root         (0)    32593 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rset.py
--rw-rw-rw-   0 root         (0) root         (0)     6543 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_rtags.py
--rw-rw-rw-   0 root         (0) root         (0)    34435 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     4051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     9574 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_uilib.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_vregistry.py
--rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/test/unittest_wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)    15556 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/toolsutils.py
--rw-rw-rw-   0 root         (0) root         (0)     3895 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/transaction.py
--rw-rw-rw-   0 root         (0) root         (0)    19495 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/uilib.py
--rw-rw-rw-   0 root         (0) root         (0)    12358 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     5113 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/wfutils.py
--rw-rw-rw-   0 root         (0) root         (0)     1578 2023-07-05 08:55:06.000000 cubicweb-4.1.0/cubicweb/xy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:36.705010 cubicweb-4.1.0/cubicweb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4231 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    51813 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      117 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      416 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-05 08:55:36.000000 cubicweb-4.1.0/cubicweb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.101015 cubicweb-4.1.0/doc/
--rw-rw-rw-   0 root         (0) root         (0)     6608 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/4.0.0_how_to_migrate.rst
--rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.101015 cubicweb-4.1.0/doc/_static/
--rw-rw-rw-   0 root         (0) root         (0)    34494 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/_static/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/_static/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/announce.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/announce.fr.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.109015 cubicweb-4.1.0/doc/api/
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/__init__.rst
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/appobject.rst
--rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/cwvreg.rst
--rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/dataimport.rst
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2536 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/predicates.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/api/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/bwcompat.rst
--rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/core.rst
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/login.rst
--rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/profile.rst
--rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/session.rst
--rw-rw-rw-   0 root         (0) root         (0)      289 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid/url_redirection.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/pyramid.rst
--rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/req.rst
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/rset.rst
--rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/urlpublishing.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/urlrewrite.rst
--rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/api/web.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/
--rw-rw-rw-   0 root         (0) root         (0)    14655 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-app.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     7806 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/_maybe_to_integrate/
--rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
--rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/rss-xml.rst
--rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/_maybe_to_integrate/template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.113015 cubicweb-4.1.0/doc/book/additionnal_services/
--rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/additionnal_services/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    13562 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/additionnal_services/undo.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.121015 cubicweb-4.1.0/doc/book/admin/
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/backups.rst
--rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/config.rst
--rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/create-instance.rst
--rw-rw-rw-   0 root         (0) root         (0)     3396 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/cubicweb-ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     4034 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/deploy.rst
--rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5172 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/instance-config.rst
--rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/ldap.rst
--rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/multisources.rst
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/rql-logs.rst
--rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/setup.rst
--rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/admin/site-config.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.121015 cubicweb-4.1.0/doc/book/annexes/
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/depends.rst
--rw-rw-rw-   0 root         (0) root         (0)     3257 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/docstrings-conventions.rst
--rw-rw-rw-   0 root         (0) root         (0)    16153 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/faq.rst
--rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3481 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/mercurial.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.125015 cubicweb-4.1.0/doc/book/annexes/rql/
--rw-rw-rw-   0 root         (0) root         (0)     2115 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/Graph-ex.gif
--rw-rw-rw-   0 root         (0) root         (0)     1167 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/debugging.rst
--rw-rw-rw-   0 root         (0) root         (0)     4697 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/implementation.rst
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5570 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/intro.rst
--rw-rw-rw-   0 root         (0) root         (0)    27490 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/language.rst
--rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/annexes/rql/usecases.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.129016 cubicweb-4.1.0/doc/book/devrepo/
--rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/connections_pooler.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.133015 cubicweb-4.1.0/doc/book/devrepo/cubes/
--rw-rw-rw-   0 root         (0) root         (0)     2645 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/available-cubes.rst
--rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/cc-newcube.rst
--rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6828 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/layout.rst
--rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/cubes/what-is-a-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/dataimport.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.133015 cubicweb-4.1.0/doc/book/devrepo/datamodel/
--rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/baseschema.rst
--rw-rw-rw-   0 root         (0) root         (0)     6178 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/define-workflows.rst
--rw-rw-rw-   0 root         (0) root         (0)    34880 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/definition.rst
--rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/datamodel/metadata.rst
--rw-rw-rw-   0 root         (0) root         (0)     2940 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/debug_channels.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.137015 cubicweb-4.1.0/doc/book/devrepo/devcore/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/devcore/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/devcore/reqbase.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.137015 cubicweb-4.1.0/doc/book/devrepo/entityclasses/
--rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/adapters.rst
--rw-rw-rw-   0 root         (0) root         (0)     7268 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/application-logic.rst
--rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/data-as-objects.rst
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1719 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/entityclasses/load-sort.rst
--rw-rw-rw-   0 root         (0) root         (0)     4399 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/fti.rst
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     9399 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/migration.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/profiling.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.141016 cubicweb-4.1.0/doc/book/devrepo/repo/
--rw-rw-rw-   0 root         (0) root         (0)     9731 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/hooks.rst
--rw-rw-rw-   0 root         (0) root         (0)      155 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/notifications.rst
--rw-rw-rw-   0 root         (0) root         (0)    11467 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/sessions.rst
--rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/repo/tasks.rst
--rw-rw-rw-   0 root         (0) root         (0)    21316 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/testing.rst
--rw-rw-rw-   0 root         (0) root         (0)    18285 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devrepo/vreg.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.145016 cubicweb-4.1.0/doc/book/devweb/
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/ajax.rst
--rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/controllers.rst
--rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/css.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.149016 cubicweb-4.1.0/doc/book/devweb/edition/
--rw-rw-rw-   0 root         (0) root         (0)    11979 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/dissection.rst
--rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/editcontroller.rst
--rw-rw-rw-   0 root         (0) root         (0)     9905 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/examples.rst
--rw-rw-rw-   0 root         (0) root         (0)    15502 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/form.rst
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/edition/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/facets.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/httpcaching.rst
--rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10057 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/internationalization.rst
--rw-rw-rw-   0 root         (0) root         (0)    14107 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/js.rst
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/property.rst
--rw-rw-rw-   0 root         (0) root         (0)     2017 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/publisher.rst
--rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/request.rst
--rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/resource.rst
--rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/rtags.rst
--rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/searchbar.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.157016 cubicweb-4.1.0/doc/book/devweb/views/
--rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/basetemplates.rst
--rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/baseviews.rst
--rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/boxes.rst
--rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/breadcrumbs.rst
--rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/idownloadable.rst
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    10179 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/primary.rst
--rw-rw-rw-   0 root         (0) root         (0)     5991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/startup.rst
--rw-rw-rw-   0 root         (0) root         (0)     5919 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/table.rst
--rw-rw-rw-   0 root         (0) root         (0)     5506 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/urlpublish.rst
--rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/views.rst
--rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/wdoc.rst
--rw-rw-rw-   0 root         (0) root         (0)     1703 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/views/xmlrss.rst
--rw-rw-rw-   0 root         (0) root         (0)      947 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/devweb/warning.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.157016 cubicweb-4.1.0/doc/book/intro/
--rw-rw-rw-   0 root         (0) root         (0)    10427 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/concepts.rst
--rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/history.rst
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/intro/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     1371 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/auth.rst
--rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/ctl.rst
--rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/debug_toolbar.rst
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1795 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/quickstart.rst
--rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/pyramid/settings.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/security/
--rw-rw-rw-   0 root         (0) root         (0)     7880 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/security/csrf.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.161016 cubicweb-4.1.0/doc/book/src/
--rw-rw-rw-   0 root         (0) root         (0)     2930 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/src/archi_globale.dia
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/book/src/main_template_layout.dia
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.173016 cubicweb-4.1.0/doc/changes/
--rw-rw-rw-   0 root         (0) root         (0)     6619 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.14.rst
--rw-rw-rw-   0 root         (0) root         (0)     3904 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.15.rst
--rw-rw-rw-   0 root         (0) root         (0)     3647 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.16.rst
--rw-rw-rw-   0 root         (0) root         (0)     1815 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.17.rst
--rw-rw-rw-   0 root         (0) root         (0)     3632 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.18.rst
--rw-rw-rw-   0 root         (0) root         (0)     6757 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.19.rst
--rw-rw-rw-   0 root         (0) root         (0)     3165 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.20.rst
--rw-rw-rw-   0 root         (0) root         (0)     2991 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.21.rst
--rw-rw-rw-   0 root         (0) root         (0)     3689 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.22.rst
--rw-rw-rw-   0 root         (0) root         (0)     2799 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.23.rst
--rw-rw-rw-   0 root         (0) root         (0)     4033 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.24.rst
--rw-rw-rw-   0 root         (0) root         (0)     4655 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.25.rst
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.26.rst
--rw-rw-rw-   0 root         (0) root         (0)     6870 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.27.rst
--rw-rw-rw-   0 root         (0) root         (0)     2656 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.28.rst
--rw-rw-rw-   0 root         (0) root         (0)     1249 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.29.rst
--rw-rw-rw-   0 root         (0) root         (0)     5588 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.30.rst
--rw-rw-rw-   0 root         (0) root         (0)     3683 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.31.rst
--rw-rw-rw-   0 root         (0) root         (0)     7979 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.32.rst
--rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.32_reledit.rst
--rw-rw-rw-   0 root         (0) root         (0)     5634 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.33.rst
--rw-rw-rw-   0 root         (0) root         (0)     4522 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.34.rst
--rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.35.rst
--rw-rw-rw-   0 root         (0) root         (0)     4486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.36.rst
--rw-rw-rw-   0 root         (0) root         (0)     5213 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.37.rst
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/3.38.rst
--rw-rw-rw-   0 root         (0) root         (0)     6422 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/4.0.rst
--rw-rw-rw-   0 root         (0) root         (0)      910 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/4.1.rst
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/changes/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     7617 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/conf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.177016 cubicweb-4.1.0/doc/dev/
--rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/coding_standards_css.rst
--rw-rw-rw-   0 root         (0) root         (0)      768 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/coding_standards_js.rst
--rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/continuous-integration.rst
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/documenting.txt
--rw-rw-rw-   0 root         (0) root         (0)    24407 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/features_list.rst
--rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/install_from_sources.rst
--rw-rw-rw-   0 root         (0) root         (0)     1241 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/dev/refactoring-the-css-with-uiprops.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/images/
--rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    12650 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/breadcrumbs_header.png
--rw-rw-rw-   0 root         (0) root         (0)    85073 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_general_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   124385 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_registry_content_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   111325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_registry_decisions_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   134505 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_rql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   192629 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_rql_traceback_panel.png
--rw-rw-rw-   0 root         (0) root         (0)   107766 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_show_source.png
--rw-rw-rw-   0 root         (0) root         (0)    55625 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_show_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)   126845 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_sql_panel.png
--rw-rw-rw-   0 root         (0) root         (0)    97343 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/debugtoolbar_traceback_source_link.png
--rw-rw-rw-   0 root         (0) root         (0)    57300 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/example-card-with-rql-directive.png
--rw-rw-rw-   0 root         (0) root         (0)    55168 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/example-card-with-rql-table-directive.png
--rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_date_range.png
--rw-rw-rw-   0 root         (0) root         (0)     6013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_has_image.png
--rw-rw-rw-   0 root         (0) root         (0)    22016 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_overview.png
--rw-rw-rw-   0 root         (0) root         (0)     1873 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/facet_range.png
--rw-rw-rw-   0 root         (0) root         (0)    21685 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_00-login_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30326 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_01-start_en.png
--rw-rw-rw-   0 root         (0) root         (0)    35859 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_02-cookie-values_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33922 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_02-create-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28123 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-list-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    82897 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-site-config-panel_en.png
--rw-rw-rw-   0 root         (0) root         (0)   119813 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-state-submitted_en.png
--rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_03-transitions-view_en.png
--rw-rw-rw-   0 root         (0) root         (0)    34771 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_04-detail-one-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    28345 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_05-list-two-blog_en.png
--rw-rw-rw-   0 root         (0) root         (0)    49230 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_06-add-relation-entryof_en.png
--rw-rw-rw-   0 root         (0) root         (0)    96838 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_06-main-template-logo_en.png
--rw-rw-rw-   0 root         (0) root         (0)    40383 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_07-detail-one-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    30591 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_08-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    33091 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_09-new-view-blogentry_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42230 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/lax-book_10-blog-with-two-entries_en.png
--rw-rw-rw-   0 root         (0) root         (0)    17757 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template.png
--rw-rw-rw-   0 root         (0) root         (0)     8674 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    13842 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/main_template_layout.png
--rw-rw-rw-   0 root         (0) root         (0)    46411 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/primaryview_template.png
--rw-rw-rw-   0 root         (0) root         (0)    14758 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/primaryview_template.svg
--rw-rw-rw-   0 root         (0) root         (0)    22773 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/request_session.png
--rw-rw-rw-   0 root         (0) root         (0)     7211 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/request_session.svg
--rw-rw-rw-   0 root         (0) root         (0)    12030 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/server-class-diagram.png
--rw-rw-rw-   0 root         (0) root         (0)    62022 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   105173 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
--rw-rw-rw-   0 root         (0) root         (0)    58500 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blog-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    42013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_blogs-list_en.png
--rw-rw-rw-   0 root         (0) root         (0)   109769 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_form-generic-relations_en.png
--rw-rw-rw-   0 root         (0) root         (0)    65646 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_en.png
--rw-rw-rw-   0 root         (0) root         (0)    13605 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_gettext_en.png
--rw-rw-rw-   0 root         (0) root         (0)    88970 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_index_logged_in_en.png
--rw-rw-rw-   0 root         (0) root         (0)    11548 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_login-form_en.png
--rw-rw-rw-   0 root         (0) root         (0)   100347 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    63097 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    62431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-default-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    74856 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
--rw-rw-rw-   0 root         (0) root         (0)    79709 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-custom-footer_en.png
--rw-rw-rw-   0 root         (0) root         (0)   128406 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    71500 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_myblog-siteinfo_en.png
--rw-rw-rw-   0 root         (0) root         (0)   104834 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_schema_en.png
--rw-rw-rw-   0 root         (0) root         (0)    22098 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_schema_graphviz_en.png
--rw-rw-rw-   0 root         (0) root         (0)   150520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-base_siteconfig_en.png
--rw-rw-rw-   0 root         (0) root         (0)    60672 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_admin.png
--rw-rw-rw-   0 root         (0) root         (0)    61388 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_city_created.png
--rw-rw-rw-   0 root         (0) root         (0)    50694 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_city_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    71561 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_data_model_schema.png
--rw-rw-rw-   0 root         (0) root         (0)    48896 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_empty_instance.png
--rw-rw-rw-   0 root         (0) root         (0)    55671 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_finished_import.png
--rw-rw-rw-   0 root         (0) root         (0)    57063 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_list_view.png
--rw-rw-rw-   0 root         (0) root         (0)    70893 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_created.png
--rw-rw-rw-   0 root         (0) root         (0)    61656 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_creation.png
--rw-rw-rw-   0 root         (0) root         (0)    74005 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_museum_with_city_name.png
--rw-rw-rw-   0 root         (0) root         (0)   225824 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_react_map.png
--rw-rw-rw-   0 root         (0) root         (0)    53544 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-museum_with_schema.png
--rw-rw-rw-   0 root         (0) root         (0)   354637 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_background-image.png
--rw-rw-rw-   0 root         (0) root         (0)    30437 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_boxes.png
--rw-rw-rw-   0 root         (0) root         (0)    54643 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_breadcrumbs.png
--rw-rw-rw-   0 root         (0) root         (0)   324086 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_facets.png
--rw-rw-rw-   0 root         (0) root         (0)    40520 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_grey-box.png
--rw-rw-rw-   0 root         (0) root         (0)    16843 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_index-after.png
--rw-rw-rw-   0 root         (0) root         (0)    26875 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_index-before.png
--rw-rw-rw-   0 root         (0) root         (0)    17580 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_login-box.png
--rw-rw-rw-   0 root         (0) root         (0)    57814 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_prevnext.png
--rw-rw-rw-   0 root         (0) root         (0)    81362 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui1.png
--rw-rw-rw-   0 root         (0) root         (0)    93291 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui2.png
--rw-rw-rw-   0 root         (0) root         (0)   290338 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/tutos-photowebsite_ui3.png
--rw-rw-rw-   0 root         (0) root         (0)    43051 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_history-view_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    26036 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_mesage_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    39625 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/undo_startup-link_w600.png
--rw-rw-rw-   0 root         (0) root         (0)    17558 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-filter-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)    14013 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-filter.png
--rw-rw-rw-   0 root         (0) root         (0)    12375 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table-shadow.png
--rw-rw-rw-   0 root         (0) root         (0)     9676 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/images/views-table.png
--rw-rw-rw-   0 root         (0) root         (0)     7225 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/plan_formation_python_cubicweb.txt
--rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/stdlib.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/tools/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/generate_modules.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/mode_plan.py
--rwxrwxrwx   0 root         (0) root         (0)     4944 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tools/pyjsrest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.241017 cubicweb-4.1.0/doc/tutorials/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.245017 cubicweb-4.1.0/doc/tutorials/advanced/
--rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     5486 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part01_create-cube.rst
--rw-rw-rw-   0 root         (0) root         (0)    17016 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part02_security.rst
--rw-rw-rw-   0 root         (0) root         (0)     5614 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part03_bfss.rst
--rw-rw-rw-   0 root         (0) root         (0)    15384 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part04_ui-base.rst
--rw-rw-rw-   0 root         (0) root         (0)    15114 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/advanced/part05_ui-advanced.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.245017 cubicweb-4.1.0/doc/tutorials/base/
--rw-rw-rw-   0 root         (0) root         (0)     3867 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/blog-in-five-minutes.rst
--rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/conclusion.rst
--rw-rw-rw-   0 root         (0) root         (0)    20431 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/customizing-the-application.rst
--rw-rw-rw-   0 root         (0) root         (0)     7821 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/discovering-the-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     1340 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/base/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.249017 cubicweb-4.1.0/doc/tutorials/dataimport/
--rw-rw-rw-   0 root         (0) root         (0)     9014 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_import.py
--rw-rw-rw-   0 root         (0) root         (0)     3336 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_parser.py
--rw-rw-rw-   0 root         (0) root         (0)    29917 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     6576 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/dataimport/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/doc/tutorials/museum/
--rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/data-management.rst
--rw-rw-rw-   0 root         (0) root         (0)     6403 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/develop-app.rst
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/develop-ui.rst
--rw-rw-rw-   0 root         (0) root         (0)     8840 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/enhance-views.rst
--rw-rw-rw-   0 root         (0) root         (0)     2702 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/getting-started.rst
--rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/museum/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/doc/tutorials/textreports/
--rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-05 08:55:06.000000 cubicweb-4.1.0/doc/tutorials/textreports/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/extras/
--rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-05 08:55:06.000000 cubicweb-4.1.0/extras/cubicweb-ctl.bash_completion
--rw-rw-rw-   0 root         (0) root         (0)     7414 2023-07-05 08:55:06.000000 cubicweb-4.1.0/jshintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.253017 cubicweb-4.1.0/man/
--rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-05 08:55:06.000000 cubicweb-4.1.0/man/cubicweb-ctl.1
--rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-05 08:55:06.000000 cubicweb-4.1.0/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-05 08:55:06.000000 cubicweb-4.1.0/pylintrc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:55:37.257017 cubicweb-4.1.0/requirements/
--rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/doc.txt
--rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/from-forge.txt
--rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-base.txt
--rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-dataimport.txt
--rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-devtools.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-ext.txt
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-hooks.txt
--rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-pyramid.txt
--rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-05 08:55:06.000000 cubicweb-4.1.0/requirements/test-server.txt
--rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-05 08:55:37.257017 cubicweb-4.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3325 2023-07-05 08:55:06.000000 cubicweb-4.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8874 2023-07-05 08:55:06.000000 cubicweb-4.1.0/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.353989 cubicweb-4.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)    17987 2023-07-25 16:23:53.000000 cubicweb-4.2.0/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)    26527 2023-07-25 16:23:53.000000 cubicweb-4.2.0/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)     4926 2023-07-25 16:23:53.000000 cubicweb-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-25 16:24:12.357989 cubicweb-4.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.969981 cubicweb-4.2.0/cubicweb/
+-rw-rw-rw-   0 root         (0) root         (0)     7348 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       69 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6885 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/_gcdebug.py
+-rw-rw-rw-   0 root         (0) root         (0)     5211 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/appobject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    64892 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    32469 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/cwgettext.py
+-rw-rw-rw-   0 root         (0) root         (0)    25984 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/cwvreg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.973981 cubicweb-4.2.0/cubicweb/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3276 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    21024 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/importer.py
+-rw-rw-rw-   0 root         (0) root         (0)    26724 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)    15511 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)    18099 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/stores.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.977981 cubicweb-4.2.0/cubicweb/dataimport/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.977981 cubicweb-4.2.0/cubicweb/dataimport/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)   474710 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/data/geonames.csv
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/data/people.csv
+-rw-rw-rw-   0 root         (0) root         (0)     1231 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    12362 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/data/timeZones.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.981982 cubicweb-4.2.0/cubicweb/dataimport/test/data-massimport/
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/data-massimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2513 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/test_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)    16178 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/test_massive_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     4179 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/test_pgstore.py
+-rw-rw-rw-   0 root         (0) root         (0)     8221 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/test_stores.py
+-rw-rw-rw-   0 root         (0) root         (0)    10720 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/dataimport/test/unittest_importer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2677 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.985982 cubicweb-4.2.0/cubicweb/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)    27150 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4116 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/apptest_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.985982 cubicweb-4.2.0/cubicweb/devtools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/data/cwmock.js
+-rw-rw-rw-   0 root         (0) root         (0)     5146 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/data/qunit.css
+-rw-rw-rw-   0 root         (0) root         (0)   115758 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/data/qunit.js
+-rw-rw-rw-   0 root         (0) root         (0)    38090 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     3702 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/fake.py
+-rw-rw-rw-   0 root         (0) root         (0)    24604 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/fill.py
+-rwxrwxrwx   0 root         (0) root         (0)     1011 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/fix_po_encoding
+-rw-rw-rw-   0 root         (0) root         (0)    10988 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/htmlparser.py
+-rw-rw-rw-   0 root         (0) root         (0)     5298 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     9217 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     2354 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/realdbtest.py
+-rw-rw-rw-   0 root         (0) root         (0)    10915 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/repotest.py
+-rw-rw-rw-   0 root         (0) root         (0)     6796 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/stresstester.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)    11311 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/firstnames.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.905980 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      462 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.989982 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/node_modules/cubes.somefile.js
+-rw-rw-rw-   0 root         (0) root         (0)     1720 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1679 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.905980 cubicweb-4.2.0/cubicweb/devtools/test/data/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.993982 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/dep_1.js
+-rw-rw-rw-   0 root         (0) root         (0)       10 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/deps_2.js
+-rw-rw-rw-   0 root         (0) root         (0)      353 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/test_simple_failure.js
+-rw-rw-rw-   0 root         (0) root         (0)      321 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/test_simple_success.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/test_with_dep.js
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/test_with_ordered_deps.js
+-rw-rw-rw-   0 root         (0) root         (0)      719 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/unittest_dbfill.py
+-rw-rw-rw-   0 root         (0) root         (0)     6402 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/unittest_devctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/unittest_fill.py
+-rw-rw-rw-   0 root         (0) root         (0)     3225 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/unittest_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/test/unittest_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)    22045 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/entities/
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24573 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/adapters.py
+-rw-rw-rw-   0 root         (0) root         (0)     6476 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/authobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4207 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     6010 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/schemaobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/sources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/entities/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/entities/test/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/entities/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1307 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9992 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/test/unittest_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    36515 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/test/unittest_wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    23208 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entities/wfobjs.py
+-rw-rw-rw-   0 root         (0) root         (0)    59296 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/ext/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5931 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/ext/html4zope.py
+-rw-rw-rw-   0 root         (0) root         (0)     1839 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/ext/markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.997982 cubicweb-4.2.0/cubicweb/ext/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2013 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/ext/test/unittest_markdown.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.001982 cubicweb-4.2.0/cubicweb/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1544 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     3089 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/email.py
+-rw-rw-rw-   0 root         (0) root         (0)    13223 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     5680 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)     9739 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     8112 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/security.py
+-rw-rw-rw-   0 root         (0) root         (0)    10642 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    60957 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4913 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2952 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/syncsources.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.005982 cubicweb-4.2.0/cubicweb/hooks/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.005982 cubicweb-4.2.0/cubicweb/hooks/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2728 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.009982 cubicweb-4.2.0/cubicweb/hooks/test/data-computed/
+-rw-rw-rw-   0 root         (0) root         (0)     1700 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/data-computed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1729 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_bookmarks.py
+-rw-rw-rw-   0 root         (0) root         (0)    13100 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     8490 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_integrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_notificationhooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2308 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     6277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_synccomputed.py
+-rw-rw-rw-   0 root         (0) root         (0)    24444 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncschema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4778 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncsession.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    15886 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/hooks/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.009982 cubicweb-4.2.0/cubicweb/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    93082 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    61668 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)   112148 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)   106920 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     3759 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     3352 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/md5crypt.py
+-rw-rw-rw-   0 root         (0) root         (0)    22356 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/migration.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.009982 cubicweb-4.2.0/cubicweb/misc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.013982 cubicweb-4.2.0/cubicweb/misc/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      690 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.22.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.22.1_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.22.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.23.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      913 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.24.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)     1412 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.24.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      117 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.27.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      217 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.30.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.31.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      423 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.32.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/3.38.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)    20222 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     3370 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/migration/postcreate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.017982 cubicweb-4.2.0/cubicweb/misc/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/scripts/chpasswd.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/scripts/detect_cycle.py
+-rw-rw-rw-   0 root         (0) root         (0)     5750 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/scripts/fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/scripts/ldap_change_base_dn.py
+-rw-rw-rw-   0 root         (0) root         (0)     3474 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/scripts/migration_helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     1097 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/misc/source_highlight.py
+-rw-rw-rw-   0 root         (0) root         (0)     3270 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/mttransforms.py
+-rw-rw-rw-   0 root         (0) root         (0)    17407 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/multipart.py
+-rw-rw-rw-   0 root         (0) root         (0)    50971 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/predicates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.021982 cubicweb-4.2.0/cubicweb/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     9374 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8851 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     4572 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     7548 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/core.py
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)     7081 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_source_code.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.025982 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/
+-rw-rw-rw-   0 root         (0) root         (0)     1895 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako
+-rw-rw-rw-   0 root         (0) root         (0)     3912 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     1592 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     4852 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     2980 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako
+-rw-rw-rw-   0 root         (0) root         (0)     8486 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/debugtoolbar_panels.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/default_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1837 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/development.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     3771 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1667 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/pyramid.ini.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)    13542 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/pyramidctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     5310 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/resources.py
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/rest_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     9634 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.025982 cubicweb-4.2.0/cubicweb/pyramid/test/
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.025982 cubicweb-4.2.0/cubicweb/pyramid/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)        5 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.029982 cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      416 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3666 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/test_config.py
+-rw-rw-rw-   0 root         (0) root         (0)     6519 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/test_content_negociation.py
+-rw-rw-rw-   0 root         (0) root         (0)      782 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/test_core.py
+-rw-rw-rw-   0 root         (0) root         (0)      986 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/test/test_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     2065 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pyramid/tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     1929 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/pytestconf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1802 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2170 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)    17499 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/req.py
+-rw-rw-rw-   0 root         (0) root         (0)    41745 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    11506 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    27303 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/rset.py
+-rw-rw-rw-   0 root         (0) root         (0)    11717 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    57984 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     6147 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schema_exporters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.029982 cubicweb-4.2.0/cubicweb/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/Bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     1696 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1662 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/_regproc.postgres.sql
+-rw-rw-rw-   0 root         (0) root         (0)    13898 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    15024 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/bootstrap.py
+-rw-rw-rw-   0 root         (0) root         (0)    11853 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/schemas/workflow.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.037983 cubicweb-4.2.0/cubicweb/server/
+-rw-rw-rw-   0 root         (0) root         (0)    14123 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3275 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/check_unused_index.py
+-rw-rw-rw-   0 root         (0) root         (0)    23459 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/checkintegrity.py
+-rw-rw-rw-   0 root         (0) root         (0)     6110 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/edition.py
+-rw-rw-rw-   0 root         (0) root         (0)    38611 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    78083 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/migractions.py
+-rw-rw-rw-   0 root         (0) root         (0)    35946 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/querier.py
+-rw-rw-rw-   0 root         (0) root         (0)    47968 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/repository.py
+-rw-rw-rw-   0 root         (0) root         (0)    19170 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    13967 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28738 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)     3168 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/serverconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)    52134 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    32452 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/session.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.041983 cubicweb-4.2.0/cubicweb/server/sources/
+-rw-rw-rw-   0 root         (0) root         (0)    13281 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18201 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    16790 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/ldapfeed.py
+-rw-rw-rw-   0 root         (0) root         (0)    78435 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/native.py
+-rw-rw-rw-   0 root         (0) root         (0)    71413 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    11169 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sources/storages.py
+-rw-rw-rw-   0 root         (0) root         (0)    22724 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    22491 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/ssplanner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.049983 cubicweb-4.2.0/cubicweb/server/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.049983 cubicweb-4.2.0/cubicweb/server/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.073983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.073983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.073983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.073983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/ldap_test.ldif
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     1585 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/slapd.conf.in
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/sources_extern
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data/sources_multi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.049983 cubicweb-4.2.0/cubicweb/server/test/data-cwep002/
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-cwep002/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.053983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.053983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.053983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.053983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.057983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.057983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.057983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.061983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.061983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.061983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.061983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.065983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.065983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.065983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.065983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.069983 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.069983 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.069983 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/
+-rw-rw-rw-   0 root         (0) root         (0)     2510 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/Company.py
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/Dates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3298 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/State.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3778 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/toignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.069983 cubicweb-4.2.0/cubicweb/server/test/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8829 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_datafeed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2192 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_edition.py
+-rw-rw-rw-   0 root         (0) root         (0)     4881 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_hook.py
+-rw-rw-rw-   0 root         (0) root         (0)    24784 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_ldapsource.py
+-rw-rw-rw-   0 root         (0) root         (0)    96667 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_querier.py
+-rw-rw-rw-   0 root         (0) root         (0)   101035 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_rql2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    23311 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_rqlannotation.py
+-rw-rw-rw-   0 root         (0) root         (0)    11087 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_schema2sql.py
+-rw-rw-rw-   0 root         (0) root         (0)    28099 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_schemaserial.py
+-rw-rw-rw-   0 root         (0) root         (0)    38100 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_server_security.py
+-rw-rw-rw-   0 root         (0) root         (0)     5431 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_server_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_serverctl.py
+-rw-rw-rw-   0 root         (0) root         (0)     2296 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_sources_native.py
+-rw-rw-rw-   0 root         (0) root         (0)     2449 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_sqlutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_ssplanner.py
+-rw-rw-rw-   0 root         (0) root         (0)    17471 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_storage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1139 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)    21794 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_undo.py
+-rw-rw-rw-   0 root         (0) root         (0)     2619 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.077983 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.081983 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.081983 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.081983 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.085984 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.085984 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.085984 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.085984 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.089984 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.089984 cubicweb-4.2.0/cubicweb/server/test_migractions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.089984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.105984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.109984 cubicweb-4.2.0/cubicweb/server/test_migractions/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.089984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.093984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.093984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.093984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.093984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.097984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.097984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.097984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.097984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.101984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.101984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.101984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.105984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.105984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.105984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.105984 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.113984 cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.113984 cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)    47835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.113984 cubicweb-4.2.0/cubicweb/server/test_migractions2/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.113984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.133985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.133985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.133985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.133985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.113984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.117984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.117984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.117984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.117984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.121984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.121984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.121984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.125985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.125985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.125985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.125985 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.129984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.129984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.129984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.129984 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9732 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions2/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.137985 cubicweb-4.2.0/cubicweb/server/test_migractions3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.141985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.157985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.161985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.161985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.161985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.161985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.165985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.165985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.141985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/
+-rw-rw-rw-   0 root         (0) root         (0)       50 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.141985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.145985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.145985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.145985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1424 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      470 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.145985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2876 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.149985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.149985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.149985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.149985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.153985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.153985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.153985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.157985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.157985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.157985 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     8437 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     9716 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.165985 cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.165985 cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1851 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1972 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_migractions3/unittest_migractions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.165985 cubicweb-4.2.0/cubicweb/server/test_postgres/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.169985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.169985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.169985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.169985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.173985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.173985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.173985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.173985 cubicweb-4.2.0/cubicweb/server/test_postgres/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)     1420 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/migration/postcreate.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/data/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    10234 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_postgres/unittest_postgres.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.177986 cubicweb-4.2.0/cubicweb/server/test_repository/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.177986 cubicweb-4.2.0/cubicweb/server/test_repository/data/
+-rw-rw-rw-   0 root         (0) root         (0)       40 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.177986 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_basket/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_basket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_basket/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      774 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.181985 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.181985 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.181985 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_file/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.181985 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.185986 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      569 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.177986 cubicweb-4.2.0/cubicweb/server/test_repository/data-schemaserial/
+-rw-rw-rw-   0 root         (0) root         (0)     1345 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data-schemaserial/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py
+-rw-rw-rw-   0 root         (0) root         (0)    37991 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/test_repository/unittest_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     5200 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/server/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.185986 cubicweb-4.2.0/cubicweb/skeleton/
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/.hgignore.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/.yamllint.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/Dockerfile.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      367 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/MANIFEST.in.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1484 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/README.rst.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.189986 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/
+-rw-rw-rw-   0 root         (0) root         (0)       97 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/__init__.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      618 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.189986 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/data/
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.css
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/data/cubes.CUBENAME.js
+-rw-rw-rw-   0 root         (0) root         (0)      190 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/entities.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      203 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/hooks.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.193986 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/i18n/fr.po
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.193986 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      425 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/postcreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      378 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/migration/precreate.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      180 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/schema.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      221 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/sobjects.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      747 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)      215 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/views.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/setup.py.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.193986 cubicweb-4.2.0/cubicweb/skeleton/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.193986 cubicweb-4.2.0/cubicweb/skeleton/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/test/data/bootstrap_cubes.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     2001 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py
+-rw-rw-rw-   0 root         (0) root         (0)     1039 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl
+-rw-rw-rw-   0 root         (0) root         (0)     1330 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/skeleton/tox.ini.tmpl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.193986 cubicweb-4.2.0/cubicweb/smoke_test/
+-rw-rw-rw-   0 root         (0) root         (0)     1433 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1455 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.197986 cubicweb-4.2.0/cubicweb/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1364 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12952 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/ldapparser.py
+-rw-rw-rw-   0 root         (0) root         (0)    14620 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5869 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/services.py
+-rw-rw-rw-   0 root         (0) root         (0)     8236 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/supervising.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.197986 cubicweb-4.2.0/cubicweb/sobjects/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.197986 cubicweb-4.2.0/cubicweb/sobjects/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       13 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.197986 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.201986 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.201986 cubicweb-4.2.0/cubicweb/sobjects/test/data/sobjects/
+-rw-rw-rw-   0 root         (0) root         (0)     1079 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/data/sobjects/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4020 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/unittest_email.py
+-rw-rw-rw-   0 root         (0) root         (0)     3061 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/unittest_notification.py
+-rw-rw-rw-   0 root         (0) root         (0)     5404 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/unittest_register_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     5051 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/sobjects/test/unittest_supervising.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/tags.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.209986 cubicweb-4.2.0/cubicweb/test/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.213986 cubicweb-4.2.0/cubicweb/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.217986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.217986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.217986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1128 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.217986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/views/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/views/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.221986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.221986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/entities/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/entities/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.221986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/hooks/
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/hooks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        7 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.221986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_forge/
+-rw-rw-rw-   0 root         (0) root         (0)      819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_forge/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.221986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_localperms/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.225986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/
+-rw-rw-rw-   0 root         (0) root         (0)      845 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      875 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/ccplugin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.225986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/
+-rw-rw-rw-   0 root         (0) root         (0)      857 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.225986 cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/erqlexpr_on_ertype.py
+-rw-rw-rw-   0 root         (0) root         (0)       77 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/lowered_etype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.229987 cubicweb-4.2.0/cubicweb/test/data/migration/
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.0.3_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.0.4_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      855 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_common.py
+-rw-rw-rw-   0 root         (0) root         (0)      847 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/migration/0.1.2_Any.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/rqlexpr_on_computedrel.py
+-rw-rw-rw-   0 root         (0) root         (0)     1555 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/rqlexpr_on_ertype_read.py
+-rw-rw-rw-   0 root         (0) root         (0)     1401 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/rrqlexpr_on_attr.py
+-rw-rw-rw-   0 root         (0) root         (0)     1182 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/rrqlexpr_on_eetype.py
+-rw-rw-rw-   0 root         (0) root         (0)     4319 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.229987 cubicweb-4.2.0/cubicweb/test/data/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/scripts/script1.py
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/scripts/script2.py
+-rw-rw-rw-   0 root         (0) root         (0)      187 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/scripts/script3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.229987 cubicweb-4.2.0/cubicweb/test/data/server_migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/server_migration/2.10.2_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/server_migration/2.5.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/server_migration/2.6.0_Any.sql
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data/uppered_rtype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.213986 cubicweb-4.2.0/cubicweb/test/data-rewrite/
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.213986 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.213986 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_localperms/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_localperms/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_localperms/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data-rewrite/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.229987 cubicweb-4.2.0/cubicweb/test/data_schemareader/
+-rw-rw-rw-   0 root         (0) root         (0)      732 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/data_schemareader/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2304 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_binary.py
+-rw-rw-rw-   0 root         (0) root         (0)      404 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_crypto.py
+-rw-rw-rw-   0 root         (0) root         (0)    17528 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_cwconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     7427 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_cwctl.py
+-rw-rw-rw-   0 root         (0) root         (0)    48020 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)     4855 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_fast_drop_entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     8359 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_mail.py
+-rw-rw-rw-   0 root         (0) root         (0)     7471 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_migration.py
+-rw-rw-rw-   0 root         (0) root         (0)    15441 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_repoapi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5855 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_req.py
+-rw-rw-rw-   0 root         (0) root         (0)    45868 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_rqlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6509 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_rqlsuggestions.py
+-rw-rw-rw-   0 root         (0) root         (0)    32593 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     6543 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_rtags.py
+-rw-rw-rw-   0 root         (0) root         (0)    34435 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     4051 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     9574 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3998 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/test/unittest_wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)    15556 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/toolsutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     3895 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/transaction.py
+-rw-rw-rw-   0 root         (0) root         (0)    19495 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/uilib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12358 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/wfutils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1578 2023-07-25 16:23:53.000000 cubicweb-4.2.0/cubicweb/xy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:11.973981 cubicweb-4.2.0/cubicweb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4231 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    51869 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      117 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      415 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-25 16:24:11.000000 cubicweb-4.2.0/cubicweb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.233986 cubicweb-4.2.0/doc/
+-rw-rw-rw-   0 root         (0) root         (0)     6763 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/4.0.0_how_to_migrate.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2811 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.233986 cubicweb-4.2.0/doc/_static/
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/_static/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/_static/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     1681 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/announce.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/announce.fr.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.237987 cubicweb-4.2.0/doc/api/
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/__init__.rst
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/appobject.rst
+-rw-rw-rw-   0 root         (0) root         (0)      830 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/cwvreg.rst
+-rw-rw-rw-   0 root         (0) root         (0)      491 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/dataimport.rst
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2536 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/predicates.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.241987 cubicweb-4.2.0/doc/api/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)      370 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/bwcompat.rst
+-rw-rw-rw-   0 root         (0) root         (0)      480 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/core.rst
+-rw-rw-rw-   0 root         (0) root         (0)      296 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/login.rst
+-rw-rw-rw-   0 root         (0) root         (0)      259 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/profile.rst
+-rw-rw-rw-   0 root         (0) root         (0)      200 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/session.rst
+-rw-rw-rw-   0 root         (0) root         (0)      289 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid/url_redirection.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/pyramid.rst
+-rw-rw-rw-   0 root         (0) root         (0)      144 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/req.rst
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/rset.rst
+-rw-rw-rw-   0 root         (0) root         (0)      781 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/urlpublishing.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/urlrewrite.rst
+-rw-rw-rw-   0 root         (0) root         (0)      520 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/api/web.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.241987 cubicweb-4.2.0/doc/book/
+-rw-rw-rw-   0 root         (0) root         (0)    14655 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/MERGE_ME-tut-create-app.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     7806 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.245987 cubicweb-4.2.0/doc/book/_maybe_to_integrate/
+-rw-rw-rw-   0 root         (0) root         (0)      225 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/_maybe_to_integrate/D050-architecture.en.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1286 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/_maybe_to_integrate/rss-xml.rst
+-rw-rw-rw-   0 root         (0) root         (0)      751 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/_maybe_to_integrate/template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.245987 cubicweb-4.2.0/doc/book/additionnal_services/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/additionnal_services/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    13562 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/additionnal_services/undo.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.249987 cubicweb-4.2.0/doc/book/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/backups.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5658 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3879 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/create-instance.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3396 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/cubicweb-ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4034 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/deploy.rst
+-rw-rw-rw-   0 root         (0) root         (0)      428 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5172 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/instance-config.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4825 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/ldap.rst
+-rw-rw-rw-   0 root         (0) root         (0)      130 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/multisources.rst
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/rql-logs.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/setup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3596 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/admin/site-config.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.249987 cubicweb-4.2.0/doc/book/annexes/
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/depends.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3257 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/docstrings-conventions.rst
+-rw-rw-rw-   0 root         (0) root         (0)    16153 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/faq.rst
+-rw-rw-rw-   0 root         (0) root         (0)      234 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/mercurial.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.253987 cubicweb-4.2.0/doc/book/annexes/rql/
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/Graph-ex.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/debugging.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4697 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/implementation.rst
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5570 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/intro.rst
+-rw-rw-rw-   0 root         (0) root         (0)    27490 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/language.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2697 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/annexes/rql/usecases.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.257987 cubicweb-4.2.0/doc/book/devrepo/
+-rw-rw-rw-   0 root         (0) root         (0)     2147 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/connections_pooler.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.257987 cubicweb-4.2.0/doc/book/devrepo/cubes/
+-rw-rw-rw-   0 root         (0) root         (0)     2645 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/cubes/available-cubes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      932 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/cubes/cc-newcube.rst
+-rw-rw-rw-   0 root         (0) root         (0)      208 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/cubes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/cubes/layout.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1967 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/cubes/what-is-a-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/dataimport.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.261987 cubicweb-4.2.0/doc/book/devrepo/datamodel/
+-rw-rw-rw-   0 root         (0) root         (0)     1389 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/datamodel/baseschema.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6178 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/datamodel/define-workflows.rst
+-rw-rw-rw-   0 root         (0) root         (0)    34880 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/datamodel/definition.rst
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/datamodel/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1043 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/datamodel/metadata.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2940 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/debug_channels.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.261987 cubicweb-4.2.0/doc/book/devrepo/devcore/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/devcore/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1129 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/devcore/reqbase.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.261987 cubicweb-4.2.0/doc/book/devrepo/entityclasses/
+-rw-rw-rw-   0 root         (0) root         (0)     5159 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/entityclasses/adapters.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7268 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/entityclasses/application-logic.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/entityclasses/data-as-objects.rst
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/entityclasses/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1719 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/entityclasses/load-sort.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4399 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/fti.rst
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9399 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/migration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/profiling.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.265987 cubicweb-4.2.0/doc/book/devrepo/repo/
+-rw-rw-rw-   0 root         (0) root         (0)     9731 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/repo/hooks.rst
+-rw-rw-rw-   0 root         (0) root         (0)      155 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/repo/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/repo/notifications.rst
+-rw-rw-rw-   0 root         (0) root         (0)    11467 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/repo/sessions.rst
+-rw-rw-rw-   0 root         (0) root         (0)       75 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/repo/tasks.rst
+-rw-rw-rw-   0 root         (0) root         (0)    21316 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/testing.rst
+-rw-rw-rw-   0 root         (0) root         (0)    18285 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devrepo/vreg.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.269987 cubicweb-4.2.0/doc/book/devweb/
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/ajax.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3473 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/controllers.rst
+-rw-rw-rw-   0 root         (0) root         (0)      890 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/css.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.269987 cubicweb-4.2.0/doc/book/devweb/edition/
+-rw-rw-rw-   0 root         (0) root         (0)    11979 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/edition/dissection.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3955 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/edition/editcontroller.rst
+-rw-rw-rw-   0 root         (0) root         (0)     9905 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/edition/examples.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15502 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/edition/form.rst
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/edition/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      698 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/facets.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/httpcaching.rst
+-rw-rw-rw-   0 root         (0) root         (0)      392 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10057 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/internationalization.rst
+-rw-rw-rw-   0 root         (0) root         (0)    14107 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/js.rst
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/property.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2017 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/publisher.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5119 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/request.rst
+-rw-rw-rw-   0 root         (0) root         (0)      709 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/resource.rst
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/rtags.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1418 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/searchbar.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.277988 cubicweb-4.2.0/doc/book/devweb/views/
+-rw-rw-rw-   0 root         (0) root         (0)     5889 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/basetemplates.rst
+-rw-rw-rw-   0 root         (0) root         (0)      701 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/baseviews.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1291 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/boxes.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/breadcrumbs.rst
+-rw-rw-rw-   0 root         (0) root         (0)      657 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/idownloadable.rst
+-rw-rw-rw-   0 root         (0) root         (0)      476 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    10179 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/primary.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5991 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)      521 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/startup.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5919 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5506 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/urlpublish.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/views.rst
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/wdoc.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1703 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/views/xmlrss.rst
+-rw-rw-rw-   0 root         (0) root         (0)      947 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/devweb/warning.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.277988 cubicweb-4.2.0/doc/book/intro/
+-rw-rw-rw-   0 root         (0) root         (0)    10427 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/intro/concepts.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1369 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/intro/history.rst
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/intro/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.281988 cubicweb-4.2.0/doc/book/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1371 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/auth.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1314 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/ctl.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3819 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/debug_toolbar.rst
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1795 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/quickstart.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/pyramid/settings.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.281988 cubicweb-4.2.0/doc/book/security/
+-rw-rw-rw-   0 root         (0) root         (0)     7880 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/security/csrf.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.281988 cubicweb-4.2.0/doc/book/src/
+-rw-rw-rw-   0 root         (0) root         (0)     2930 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/src/archi_globale.dia
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/book/src/main_template_layout.dia
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.293988 cubicweb-4.2.0/doc/changes/
+-rw-rw-rw-   0 root         (0) root         (0)     6619 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.14.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3904 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.15.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.16.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1815 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.17.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3632 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.18.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6757 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.19.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3165 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.20.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2991 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.21.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3689 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.22.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2799 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.23.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4033 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.24.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4655 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.25.rst
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.26.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6870 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.27.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2656 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.28.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1249 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.29.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5588 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.30.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.31.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7979 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.32.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1728 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.32_reledit.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5634 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.33.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4522 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.34.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.35.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4486 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.36.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5411 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.37.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7538 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/3.38.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6422 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/4.0.rst
+-rw-rw-rw-   0 root         (0) root         (0)      910 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/4.1.rst
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/4.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)      641 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/changes/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7617 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/conf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.293988 cubicweb-4.2.0/doc/dev/
+-rw-rw-rw-   0 root         (0) root         (0)      708 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/coding_standards_css.rst
+-rw-rw-rw-   0 root         (0) root         (0)      768 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/coding_standards_js.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1037 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/continuous-integration.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/documenting.txt
+-rw-rw-rw-   0 root         (0) root         (0)    24407 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/features_list.rst
+-rw-rw-rw-   0 root         (0) root         (0)      253 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/install_from_sources.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/dev/refactoring-the-css-with-uiprops.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.341989 cubicweb-4.2.0/doc/images/
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    12650 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/breadcrumbs_header.png
+-rw-rw-rw-   0 root         (0) root         (0)    85073 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_general_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   124385 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_registry_content_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   111325 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_registry_decisions_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   134505 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_rql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   192629 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_rql_traceback_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)   107766 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_show_source.png
+-rw-rw-rw-   0 root         (0) root         (0)    55625 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_show_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)   126845 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_sql_panel.png
+-rw-rw-rw-   0 root         (0) root         (0)    97343 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/debugtoolbar_traceback_source_link.png
+-rw-rw-rw-   0 root         (0) root         (0)    57300 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/example-card-with-rql-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)    55168 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/example-card-with-rql-table-directive.png
+-rw-rw-rw-   0 root         (0) root         (0)     2277 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/facet_date_range.png
+-rw-rw-rw-   0 root         (0) root         (0)     6013 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/facet_has_image.png
+-rw-rw-rw-   0 root         (0) root         (0)    22016 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/facet_overview.png
+-rw-rw-rw-   0 root         (0) root         (0)     1873 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/facet_range.png
+-rw-rw-rw-   0 root         (0) root         (0)    21685 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_00-login_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30326 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_01-start_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    35859 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_02-cookie-values_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33922 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_02-create-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28123 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_03-list-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    82897 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_03-site-config-panel_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   119813 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_03-state-submitted_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    98393 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_03-transitions-view_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    34771 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_04-detail-one-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    28345 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_05-list-two-blog_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    49230 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_06-add-relation-entryof_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    96838 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_06-main-template-logo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    40383 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_07-detail-one-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    30591 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_08-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    33091 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_09-new-view-blogentry_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42230 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/lax-book_10-blog-with-two-entries_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    17757 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/main_template.png
+-rw-rw-rw-   0 root         (0) root         (0)     8674 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/main_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    13842 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/main_template_layout.png
+-rw-rw-rw-   0 root         (0) root         (0)    46411 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/primaryview_template.png
+-rw-rw-rw-   0 root         (0) root         (0)    14758 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/primaryview_template.svg
+-rw-rw-rw-   0 root         (0) root         (0)    22773 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/request_session.png
+-rw-rw-rw-   0 root         (0) root         (0)     7211 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/request_session.svg
+-rw-rw-rw-   0 root         (0) root         (0)    12030 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/server-class-diagram.png
+-rw-rw-rw-   0 root         (0) root         (0)    62022 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_blog-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   105173 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    58500 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_blog-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    42013 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_blogs-list_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   109769 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_form-generic-relations_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    65646 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_index_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    13605 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_index_gettext_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    88970 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_index_logged_in_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    11548 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_login-form_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   100347 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    63097 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-community-custom-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    62431 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-community-default-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    74856 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    79709 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-custom-footer_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   128406 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    71500 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_myblog-siteinfo_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   104834 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_schema_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    22098 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_schema_graphviz_en.png
+-rw-rw-rw-   0 root         (0) root         (0)   150520 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-base_siteconfig_en.png
+-rw-rw-rw-   0 root         (0) root         (0)    60672 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_admin.png
+-rw-rw-rw-   0 root         (0) root         (0)    61388 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_city_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    50694 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_city_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    71561 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_data_model_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)    48896 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_empty_instance.png
+-rw-rw-rw-   0 root         (0) root         (0)    55671 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_finished_import.png
+-rw-rw-rw-   0 root         (0) root         (0)    57063 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_list_view.png
+-rw-rw-rw-   0 root         (0) root         (0)    70893 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_museum_created.png
+-rw-rw-rw-   0 root         (0) root         (0)    61656 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_museum_creation.png
+-rw-rw-rw-   0 root         (0) root         (0)    74005 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_museum_with_city_name.png
+-rw-rw-rw-   0 root         (0) root         (0)   225824 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_react_map.png
+-rw-rw-rw-   0 root         (0) root         (0)    53544 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-museum_with_schema.png
+-rw-rw-rw-   0 root         (0) root         (0)   354637 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_background-image.png
+-rw-rw-rw-   0 root         (0) root         (0)    30437 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_boxes.png
+-rw-rw-rw-   0 root         (0) root         (0)    54643 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_breadcrumbs.png
+-rw-rw-rw-   0 root         (0) root         (0)   324086 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_facets.png
+-rw-rw-rw-   0 root         (0) root         (0)    40520 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_grey-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    16843 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_index-after.png
+-rw-rw-rw-   0 root         (0) root         (0)    26875 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_index-before.png
+-rw-rw-rw-   0 root         (0) root         (0)    17580 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_login-box.png
+-rw-rw-rw-   0 root         (0) root         (0)    57814 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_prevnext.png
+-rw-rw-rw-   0 root         (0) root         (0)    81362 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_ui1.png
+-rw-rw-rw-   0 root         (0) root         (0)    93291 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_ui2.png
+-rw-rw-rw-   0 root         (0) root         (0)   290338 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/tutos-photowebsite_ui3.png
+-rw-rw-rw-   0 root         (0) root         (0)    43051 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/undo_history-view_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    26036 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/undo_mesage_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    39625 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/undo_startup-link_w600.png
+-rw-rw-rw-   0 root         (0) root         (0)    17558 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/views-table-filter-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)    14013 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/views-table-filter.png
+-rw-rw-rw-   0 root         (0) root         (0)    12375 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/views-table-shadow.png
+-rw-rw-rw-   0 root         (0) root         (0)     9676 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/images/views-table.png
+-rw-rw-rw-   0 root         (0) root         (0)     7225 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2011 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/plan_formation_python_cubicweb.txt
+-rw-rw-rw-   0 root         (0) root         (0)      139 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/stdlib.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.341989 cubicweb-4.2.0/doc/tools/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tools/generate_modules.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tools/mode_plan.py
+-rwxrwxrwx   0 root         (0) root         (0)     4944 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tools/pyjsrest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.341989 cubicweb-4.2.0/doc/tutorials/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.345989 cubicweb-4.2.0/doc/tutorials/advanced/
+-rw-rw-rw-   0 root         (0) root         (0)      604 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5486 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/part01_create-cube.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17016 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/part02_security.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5614 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/part03_bfss.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15384 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/part04_ui-base.rst
+-rw-rw-rw-   0 root         (0) root         (0)    15114 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/advanced/part05_ui-advanced.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.345989 cubicweb-4.2.0/doc/tutorials/base/
+-rw-rw-rw-   0 root         (0) root         (0)     3867 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/base/blog-in-five-minutes.rst
+-rw-rw-rw-   0 root         (0) root         (0)      675 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/base/conclusion.rst
+-rw-rw-rw-   0 root         (0) root         (0)    20431 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/base/customizing-the-application.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7821 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/base/discovering-the-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1340 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/base/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.349989 cubicweb-4.2.0/doc/tutorials/dataimport/
+-rw-rw-rw-   0 root         (0) root         (0)     9014 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/dataimport/diseasome_import.py
+-rw-rw-rw-   0 root         (0) root         (0)     3336 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/dataimport/diseasome_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)    29917 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/dataimport/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6576 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/dataimport/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.349989 cubicweb-4.2.0/doc/tutorials/museum/
+-rw-rw-rw-   0 root         (0) root         (0)     5961 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/data-management.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6403 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/develop-app.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/develop-ui.rst
+-rw-rw-rw-   0 root         (0) root         (0)     8840 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/enhance-views.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2702 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/getting-started.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1595 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/museum/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.349989 cubicweb-4.2.0/doc/tutorials/textreports/
+-rw-rw-rw-   0 root         (0) root         (0)      440 2023-07-25 16:23:53.000000 cubicweb-4.2.0/doc/tutorials/textreports/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.349989 cubicweb-4.2.0/extras/
+-rw-rw-rw-   0 root         (0) root         (0)     3545 2023-07-25 16:23:53.000000 cubicweb-4.2.0/extras/cubicweb-ctl.bash_completion
+-rw-rw-rw-   0 root         (0) root         (0)     7414 2023-07-25 16:23:53.000000 cubicweb-4.2.0/jshintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.353989 cubicweb-4.2.0/man/
+-rw-rw-rw-   0 root         (0) root         (0)      651 2023-07-25 16:23:53.000000 cubicweb-4.2.0/man/cubicweb-ctl.1
+-rw-rw-rw-   0 root         (0) root         (0)       56 2023-07-25 16:23:53.000000 cubicweb-4.2.0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)      536 2023-07-25 16:23:53.000000 cubicweb-4.2.0/pylintrc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-25 16:24:12.353989 cubicweb-4.2.0/requirements/
+-rw-rw-rw-   0 root         (0) root         (0)      174 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      377 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/from-forge.txt
+-rw-rw-rw-   0 root         (0) root         (0)      380 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-base.txt
+-rw-rw-rw-   0 root         (0) root         (0)       16 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-dataimport.txt
+-rw-rw-rw-   0 root         (0) root         (0)       15 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-devtools.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-ext.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-hooks.txt
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-pyramid.txt
+-rw-rw-rw-   0 root         (0) root         (0)       35 2023-07-25 16:23:53.000000 cubicweb-4.2.0/requirements/test-server.txt
+-rw-rw-rw-   0 root         (0) root         (0)      115 2023-07-25 16:24:12.357989 cubicweb-4.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3324 2023-07-25 16:23:53.000000 cubicweb-4.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8874 2023-07-25 16:23:53.000000 cubicweb-4.2.0/tox.ini
```

### Comparing `cubicweb-4.1.0/COPYING` & `cubicweb-4.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/COPYING.LESSER` & `cubicweb-4.2.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/MANIFEST.in` & `cubicweb-4.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/PKG-INFO` & `cubicweb-4.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.1.0
+Version: 4.2.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 Provides-Extra: captcha
```

### Comparing `cubicweb-4.1.0/README.rst` & `cubicweb-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/__init__.py` & `cubicweb-4.2.0/cubicweb/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/__pkginfo__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """cubicweb global packaging information for the cubicweb knowledge management
 software
 """
 
 modname = distname = "cubicweb"
 
-numversion = (4, 1, 0)
+numversion = (4, 2, 0)
 version = ".".join(str(num) for num in numversion)
 
 description = "a repository of entities / relations for knowledge management"
 author = "Logilab"
 author_email = "contact@logilab.fr"
 web = "https://www.cubicweb.org"
 license = "LGPL"
```

### Comparing `cubicweb-4.1.0/cubicweb/_exceptions.py` & `cubicweb-4.2.0/cubicweb/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/_gcdebug.py` & `cubicweb-4.2.0/cubicweb/_gcdebug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/appobject.py` & `cubicweb-4.2.0/cubicweb/appobject.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/crypto.py` & `cubicweb-4.2.0/cubicweb/crypto.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/cwconfig.py` & `cubicweb-4.2.0/cubicweb/cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/cwctl.py` & `cubicweb-4.2.0/cubicweb/cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/cwgettext.py` & `cubicweb-4.2.0/cubicweb/cwgettext.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/cwvreg.py` & `cubicweb-4.2.0/cubicweb/cwvreg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/__init__.py` & `cubicweb-4.2.0/cubicweb/dataimport/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/csv.py` & `cubicweb-4.2.0/cubicweb/dataimport/csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/importer.py` & `cubicweb-4.2.0/cubicweb/dataimport/importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/massive_store.py` & `cubicweb-4.2.0/cubicweb/dataimport/massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/pgstore.py` & `cubicweb-4.2.0/cubicweb/dataimport/pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/stores.py` & `cubicweb-4.2.0/cubicweb/dataimport/stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/data/geonames.csv` & `cubicweb-4.2.0/cubicweb/dataimport/test/data/geonames.csv`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/data/timeZones.txt` & `cubicweb-4.2.0/cubicweb/dataimport/test/data/timeZones.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/data-massimport/schema.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/data-massimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/test_csv.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/test_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/test_massive_store.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/test_massive_store.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/test_pgstore.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/test_pgstore.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/test_stores.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/test_stores.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/dataimport/test/unittest_importer.py` & `cubicweb-4.2.0/cubicweb/dataimport/test/unittest_importer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/debug.py` & `cubicweb-4.2.0/cubicweb/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/__init__.py` & `cubicweb-4.2.0/cubicweb/devtools/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/apptest_config.py` & `cubicweb-4.2.0/cubicweb/devtools/apptest_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/data/qunit.css` & `cubicweb-4.2.0/cubicweb/devtools/data/qunit.css`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/data/qunit.js` & `cubicweb-4.2.0/cubicweb/devtools/data/qunit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/devctl.py` & `cubicweb-4.2.0/cubicweb/devtools/devctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/fake.py` & `cubicweb-4.2.0/cubicweb/devtools/fake.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/fill.py` & `cubicweb-4.2.0/cubicweb/devtools/fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/fix_po_encoding` & `cubicweb-4.2.0/cubicweb/devtools/fix_po_encoding`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/htmlparser.py` & `cubicweb-4.2.0/cubicweb/devtools/htmlparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/httptest.py` & `cubicweb-4.2.0/cubicweb/devtools/httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/instrument.py` & `cubicweb-4.2.0/cubicweb/devtools/instrument.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/realdbtest.py` & `cubicweb-4.2.0/cubicweb/devtools/realdbtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/repotest.py` & `cubicweb-4.2.0/cubicweb/devtools/repotest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/stresstester.py` & `cubicweb-4.2.0/cubicweb/devtools/stresstester.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2023 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact https://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of CubicWeb.
 #
 # CubicWeb is free software: you can redistribute it and/or modify it under the
 # terms of the GNU Lesser General Public License as published by the Free
 # Software Foundation, either version 2.1 of the License, or (at your option)
@@ -34,25 +34,25 @@
   -t / --nb-threads <num>
      Execute queries in <num> parallel threads.
   -P / --profile <prof_file>
      dumps profile results (hotshot) in <prof_file>
   -o / --report-output <filename>
      Write profiler report into <filename> rather than on stdout
 
-Copyright (c) 2003-2011 LOGILAB S.A. (Paris, FRANCE), license is LGPL v2.
+Copyright (c) 2003-2023 LOGILAB S.A. (Paris, FRANCE), license is LGPL v2.
 https://www.logilab.fr/ -- mailto:contact@logilab.fr
 """
 import getopt
 import os
 import sys
 import threading
 import traceback
 from getpass import getpass
 from os.path import basename
-from time import clock
+from time import process_time
 
 from logilab.common.fileutils import lines
 from logilab.common.ureports import Table, TextWriter
 
 from cubicweb import repoapi
 from cubicweb.server.repository import Repository
 
@@ -67,24 +67,24 @@
         self._reporter = reporter
 
     def run(self):
         with self._cnx as cnx:
             times = self._times
             while times:
                 for index, query in enumerate(self._queries):
-                    start = clock()
+                    start = process_time()
                     try:
                         cnx.execute(query)
                     except Exception:
                         TB_LOCK.acquire()
                         traceback.print_exc()
                         TB_LOCK.release()
                         return
                     if self._reporter is not None:
-                        self._reporter.add_proftime(clock() - start, index)
+                        self._reporter.add_proftime(process_time() - start, index)
                 times -= 1
 
 
 def usage(status=0):
     """print usage string and exit"""
     print(__doc__ % basename(sys.argv[0]))
     sys.exit(status)
```

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/data/firstnames.txt` & `cubicweb-4.2.0/cubicweb/devtools/test/data/firstnames.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-4.2.0/cubicweb/devtools/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/devtools/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/data/static/js_examples/utils.js` & `cubicweb-4.2.0/cubicweb/devtools/test/data/static/js_examples/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/unittest_dbfill.py` & `cubicweb-4.2.0/cubicweb/devtools/test/unittest_dbfill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/unittest_devctl.py` & `cubicweb-4.2.0/cubicweb/devtools/test/unittest_devctl.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,18 @@
             # use a fake HOME).
             env["PYTHONPATH"] = user_site
             cmd = [sys.executable, "setup.py", "install", "--user"]
             proc = Popen(cmd, stdout=PIPE, stderr=STDOUT, cwd=projectdir, env=env)
             retcode = proc.wait()
             stdout = to_unicode(proc.stdout.read())
             self.assertEqual(retcode, 0, stdout)
-            target_egg = "cubicweb_foo-0.1.0-py{}.egg".format(sys.version[:3]).encode()
+            version = sys.version_info
+            target_egg = (
+                f"cubicweb_foo-0.1.0-py{version.major}.{version.minor}.egg".encode()
+            )
             self.assertTrue(
                 osp.isdir(osp.join(user_site, target_egg)),
                 f"target: '{target_egg}', target directory content: {os.listdir(user_site)}",
             )
             pkgdir = osp.join(user_site, target_egg, b"cubicweb_foo")
             self.assertTrue(
                 osp.isdir(pkgdir), os.listdir(osp.join(user_site, target_egg))
```

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/unittest_fill.py` & `cubicweb-4.2.0/cubicweb/devtools/test/unittest_fill.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/unittest_i18n.py` & `cubicweb-4.2.0/cubicweb/devtools/test/unittest_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/test/unittest_testlib.py` & `cubicweb-4.2.0/cubicweb/devtools/test/unittest_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/devtools/testlib.py` & `cubicweb-4.2.0/cubicweb/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/__init__.py` & `cubicweb-4.2.0/cubicweb/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/adapters.py` & `cubicweb-4.2.0/cubicweb/entities/adapters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/authobjs.py` & `cubicweb-4.2.0/cubicweb/entities/authobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/lib.py` & `cubicweb-4.2.0/cubicweb/entities/lib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/schemaobjs.py` & `cubicweb-4.2.0/cubicweb/entities/schemaobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/sources.py` & `cubicweb-4.2.0/cubicweb/entities/sources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/test/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/entities/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/entities/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/test/unittest_base.py` & `cubicweb-4.2.0/cubicweb/entities/test/unittest_base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/test/unittest_wfobjs.py` & `cubicweb-4.2.0/cubicweb/entities/test/unittest_wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entities/wfobjs.py` & `cubicweb-4.2.0/cubicweb/entities/wfobjs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/entity.py` & `cubicweb-4.2.0/cubicweb/entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/ext/__init__.py` & `cubicweb-4.2.0/cubicweb/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/ext/html4zope.py` & `cubicweb-4.2.0/cubicweb/ext/html4zope.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/ext/markdown.py` & `cubicweb-4.2.0/cubicweb/ext/markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/ext/test/unittest_markdown.py` & `cubicweb-4.2.0/cubicweb/ext/test/unittest_markdown.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/__init__.py` & `cubicweb-4.2.0/cubicweb/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/bookmark.py` & `cubicweb-4.2.0/cubicweb/hooks/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/email.py` & `cubicweb-4.2.0/cubicweb/hooks/email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/integrity.py` & `cubicweb-4.2.0/cubicweb/hooks/integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/metadata.py` & `cubicweb-4.2.0/cubicweb/hooks/metadata.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/notification.py` & `cubicweb-4.2.0/cubicweb/hooks/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/security.py` & `cubicweb-4.2.0/cubicweb/hooks/security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/synccomputed.py` & `cubicweb-4.2.0/cubicweb/hooks/synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/syncschema.py` & `cubicweb-4.2.0/cubicweb/hooks/syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/syncsession.py` & `cubicweb-4.2.0/cubicweb/hooks/syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/syncsources.py` & `cubicweb-4.2.0/cubicweb/hooks/syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/hooks/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/data-computed/schema.py` & `cubicweb-4.2.0/cubicweb/hooks/test/data-computed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_bookmarks.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_bookmarks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_hooks.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_integrity.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_integrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_notificationhooks.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_notificationhooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_security.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_synccomputed.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_synccomputed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncschema.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncschema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsession.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncsession.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/test/unittest_syncsources.py` & `cubicweb-4.2.0/cubicweb/hooks/test/unittest_syncsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/hooks/workflow.py` & `cubicweb-4.2.0/cubicweb/hooks/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/i18n/de.po` & `cubicweb-4.2.0/cubicweb/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/i18n/en.po` & `cubicweb-4.2.0/cubicweb/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/i18n/es.po` & `cubicweb-4.2.0/cubicweb/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/i18n/fr.po` & `cubicweb-4.2.0/cubicweb/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/i18n.py` & `cubicweb-4.2.0/cubicweb/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/mail.py` & `cubicweb-4.2.0/cubicweb/mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/md5crypt.py` & `cubicweb-4.2.0/cubicweb/md5crypt.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/migration.py` & `cubicweb-4.2.0/cubicweb/migration.py`

 * *Files 1% similar despite different names*

```diff
@@ -440,29 +440,34 @@
             cubes = (cubes,)
         origcubes = self.config.cubes()
         newcubes = [p for p in self.config.expand_cubes(cubes) if p not in origcubes]
         if newcubes:
             self.config.add_cubes(newcubes)
         return newcubes
 
-    def cmd_drop_cube(self, cube, removedeps=False):
+    def cmd_drop_cube(self, cube, removedeps=False, force_drop=False):
         if removedeps:
             toremove = self.config.expand_cubes([cube])
         else:
             toremove = (cube,)
         origcubes = self.config._cubes
         basecubes = [c for c in origcubes if c not in toremove]
         # don't fake-add any new ones, or we won't be able to really-add them later
-        self.config._cubes = tuple(
-            cube for cube in self.config.expand_cubes(basecubes) if cube in origcubes
-        )
+        new_config_cubes = []
+        for c in self.config.expand_cubes(basecubes):
+            if c in origcubes:
+                if c in toremove and force_drop:
+                    continue
+                new_config_cubes.append(c)
+        self.config._cubes = tuple(new_config_cubes)
         removed = [p for p in origcubes if p not in self.config._cubes]
         if cube not in removed and cube in origcubes:
             raise ConfigurationError(
-                "can't remove cube %s, " "used as a dependency" % cube
+                f"can't remove cube {cube}, used as a dependency."
+                f"Consider using 'force_drop=True' if you want to drop it anyway"
             )
         return removed
 
     def rewrite_configuration(self):
         configfile = self.config.main_config_file()
         if self._option_changes:
             read_old_config(self.config, self._option_changes, configfile)
```

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/3.22.0_Any.py` & `cubicweb-4.2.0/cubicweb/misc/migration/3.22.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/3.23.0_Any.py` & `cubicweb-4.2.0/cubicweb/misc/migration/3.23.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/3.24.0_Any.py` & `cubicweb-4.2.0/cubicweb/misc/migration/3.24.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/3.24.4_Any.py` & `cubicweb-4.2.0/cubicweb/misc/migration/3.24.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/bootstrapmigration_repository.py` & `cubicweb-4.2.0/cubicweb/misc/migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/misc/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/scripts/chpasswd.py` & `cubicweb-4.2.0/cubicweb/misc/scripts/chpasswd.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/scripts/fast_drop_entities.py` & `cubicweb-4.2.0/cubicweb/misc/scripts/fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/scripts/ldap_change_base_dn.py` & `cubicweb-4.2.0/cubicweb/misc/scripts/ldap_change_base_dn.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/scripts/migration_helper.py` & `cubicweb-4.2.0/cubicweb/misc/scripts/migration_helper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/misc/source_highlight.py` & `cubicweb-4.2.0/cubicweb/misc/source_highlight.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/mttransforms.py` & `cubicweb-4.2.0/cubicweb/mttransforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/multipart.py` & `cubicweb-4.2.0/cubicweb/multipart.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/predicates.py` & `cubicweb-4.2.0/cubicweb/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/__init__.py` & `cubicweb-4.2.0/cubicweb/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/auth.py` & `cubicweb-4.2.0/cubicweb/pyramid/auth.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/config.py` & `cubicweb-4.2.0/cubicweb/pyramid/config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/core.py` & `cubicweb-4.2.0/cubicweb/pyramid/core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/csrf.py` & `cubicweb-4.2.0/cubicweb/pyramid/csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_source_code.py` & `cubicweb-4.2.0/cubicweb/pyramid/debug_source_code.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/cw.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/debug_source_code.mako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/registry.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/registry_decisions.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/rql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako` & `cubicweb-4.2.0/cubicweb/pyramid/debug_toolbar_templates/sql.dbtmako`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/debugtoolbar_panels.py` & `cubicweb-4.2.0/cubicweb/pyramid/debugtoolbar_panels.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/development.ini.tmpl` & `cubicweb-4.2.0/cubicweb/pyramid/development.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/predicates.py` & `cubicweb-4.2.0/cubicweb/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/pyramid.ini.tmpl` & `cubicweb-4.2.0/cubicweb/pyramid/pyramid.ini.tmpl`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 #   since cubicweb_web provides better ones.
 #   To disable html default views, comment "cubicweb.pyramid.rest_api.include_html". To
 #   disable RDF default views, comment "cubicweb.pyramid.rest_api.include_rdf".
 
 cubicweb.includes =
   # Warning: Everything added here will be added before every includeme of every cubes.
   cubicweb.pyramid.auth
+  cubicweb.pyramid.default_session
   # cubicweb.pyramid.session
   # Add views to generate one html page per entity
   cubicweb.pyramid.rest_api.include_html
   # Add views to generate one RDF graph per entity
   cubicweb.pyramid.rest_api.include_rdf
   # Add views to download entities adaptable to IDownloadable
   cubicweb.pyramid.rest_api.include_download
```

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/pyramidctl.py` & `cubicweb-4.2.0/cubicweb/pyramid/pyramidctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/resources.py` & `cubicweb-4.2.0/cubicweb/pyramid/resources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/rest_api.py` & `cubicweb-4.2.0/cubicweb/pyramid/rest_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/session.py` & `cubicweb-4.2.0/cubicweb/pyramid/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/__init__.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/test_config.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/test_config.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/test_content_negociation.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/test_content_negociation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/test_core.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/test_core.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/test/test_tools.py` & `cubicweb-4.2.0/cubicweb/pyramid/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pyramid/tools.py` & `cubicweb-4.2.0/cubicweb/pyramid/tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/pytestconf.py` & `cubicweb-4.2.0/cubicweb/pytestconf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/rdf.py` & `cubicweb-4.2.0/cubicweb/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/repoapi.py` & `cubicweb-4.2.0/cubicweb/repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/req.py` & `cubicweb-4.2.0/cubicweb/req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/rqlrewrite.py` & `cubicweb-4.2.0/cubicweb/rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/rqlsuggestions.py` & `cubicweb-4.2.0/cubicweb/rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/rset.py` & `cubicweb-4.2.0/cubicweb/rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/rtags.py` & `cubicweb-4.2.0/cubicweb/rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schema.py` & `cubicweb-4.2.0/cubicweb/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schema_exporters.py` & `cubicweb-4.2.0/cubicweb/schema_exporters.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/Bookmark.py` & `cubicweb-4.2.0/cubicweb/schemas/Bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/__init__.py` & `cubicweb-4.2.0/cubicweb/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/_regproc.postgres.sql` & `cubicweb-4.2.0/cubicweb/schemas/_regproc.postgres.sql`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/base.py` & `cubicweb-4.2.0/cubicweb/schemas/base.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/bootstrap.py` & `cubicweb-4.2.0/cubicweb/schemas/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/schemas/workflow.py` & `cubicweb-4.2.0/cubicweb/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/__init__.py` & `cubicweb-4.2.0/cubicweb/server/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/check_unused_index.py` & `cubicweb-4.2.0/cubicweb/server/check_unused_index.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/checkintegrity.py` & `cubicweb-4.2.0/cubicweb/server/checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/edition.py` & `cubicweb-4.2.0/cubicweb/server/edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/hook.py` & `cubicweb-4.2.0/cubicweb/server/hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/migractions.py` & `cubicweb-4.2.0/cubicweb/server/migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/querier.py` & `cubicweb-4.2.0/cubicweb/server/querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/repository.py` & `cubicweb-4.2.0/cubicweb/server/repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/rqlannotation.py` & `cubicweb-4.2.0/cubicweb/server/rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/schema2sql.py` & `cubicweb-4.2.0/cubicweb/server/schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/schemaserial.py` & `cubicweb-4.2.0/cubicweb/server/schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/serverconfig.py` & `cubicweb-4.2.0/cubicweb/server/serverconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/serverctl.py` & `cubicweb-4.2.0/cubicweb/server/serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/session.py` & `cubicweb-4.2.0/cubicweb/server/session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/__init__.py` & `cubicweb-4.2.0/cubicweb/server/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/datafeed.py` & `cubicweb-4.2.0/cubicweb/server/sources/datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/ldapfeed.py` & `cubicweb-4.2.0/cubicweb/server/sources/ldapfeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/native.py` & `cubicweb-4.2.0/cubicweb/server/sources/native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/rql2sql.py` & `cubicweb-4.2.0/cubicweb/server/sources/rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sources/storages.py` & `cubicweb-4.2.0/cubicweb/server/sources/storages.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/sqlutils.py` & `cubicweb-4.2.0/cubicweb/server/sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/ssplanner.py` & `cubicweb-4.2.0/cubicweb/server/ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/ldap_test.ldif` & `cubicweb-4.2.0/cubicweb/server/test/data/ldap_test.ldif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data/slapd.conf.in` & `cubicweb-4.2.0/cubicweb/server/test/data/slapd.conf.in`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-cwep002/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-cwep002/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-migractions/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Company.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/Company.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/Dates.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/Dates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/State.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/State.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/__init__.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schema2sql/schema/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schema2sql/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/datacomputed/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/datacomputed/schema.py` & `cubicweb-4.2.0/cubicweb/server/test/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_datafeed.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_datafeed.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_edition.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_edition.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_hook.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_hook.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_ldapsource.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_ldapsource.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,16 @@
     config.info("Initing ldap database")
     cmdline = ["/usr/sbin/slapadd", "-f", slapdconf, "-l", ldiffile, "-c"]
     PIPE = subprocess.PIPE
     slapproc = subprocess.Popen(cmdline, stdout=PIPE, stderr=PIPE)
     stdout, stderr = slapproc.communicate()
     if slapproc.returncode:
         print("slapadd returned with status: %s" % slapproc.returncode, file=sys.stderr)
-        sys.stdout.write(stdout)
-        sys.stderr.write(stderr)
+        sys.stdout.write(stdout.decode())
+        sys.stderr.write(stderr.decode())
 
     # ldapuri = 'ldapi://' + join(basedir, "ldapi").replace('/', '%2f')
     port = get_available_port(range(9000, 9100))
     host = "localhost:%s" % port
     ldapuri = "ldap://%s" % host
     cmdline = ["/usr/sbin/slapd", "-f", slapdconf, "-h", ldapuri, "-d", "0"]
     config.info("Starting slapd:", " ".join(cmdline))
```

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_querier.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_querier.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_rql2sql.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_rql2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_rqlannotation.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_rqlannotation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_schema2sql.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_schema2sql.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_schemaserial.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_schemaserial.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_server_security.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_server_security.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_server_utils.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_server_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_serverctl.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_serverctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_session.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_session.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_sources_native.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_sources_native.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_sqlutils.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_sqlutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_ssplanner.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_ssplanner.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_storage.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_storage.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_tools.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_tools.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_undo.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_undo.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test/unittest_utils.py` & `cubicweb-4.2.0/cubicweb/server/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py` & `cubicweb-4.2.0/cubicweb/server/test_checkintegrity/unittest_checkintegrity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/data-migractions/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/datacomputed/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions/unittest_migractions.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions/unittest_migractions.py`

 * *Files 1% similar despite different names*

```diff
@@ -933,15 +933,17 @@
                 cnx.commit()
 
     def test_drop_dep_cube(self):
         with self.mh() as (cnx, mh):
             with self.assertRaises(ConfigurationError) as cm:
                 mh.cmd_drop_cube("file")
             self.assertEqual(
-                str(cm.exception), "can't remove cube file, used as a dependency"
+                str(cm.exception),
+                "can't remove cube file, used as a dependency."
+                "Consider using 'force_drop=True' if you want to drop it anyway",
             )
 
     def test_introduce_base_class(self):
         with self.mh() as (cnx, mh):
             mh.cmd_add_entity_type("Para")
             self.assertEqual(
                 sorted(et.type for et in self.schema["Para"].specialized_by()), ["Note"]
```

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/data-migractions/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/datacomputed/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions2/unittest_migractions.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions2/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakecustomtype/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_fakeemail/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/data-migractions/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/data-migractions/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/migratedapp/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/datacomputed/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/datacomputed/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_migractions3/unittest_migractions.py` & `cubicweb-4.2.0/cubicweb/server/test_migractions3/unittest_migractions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/migration/postcreate.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/migration/postcreate.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_postgres/unittest_postgres.py` & `cubicweb-4.2.0/cubicweb/server/test_postgres/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_basket/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/entities.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/hooks.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/schema.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data-schemaserial/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/data-schemaserial/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/test_repository/unittest_repository.py` & `cubicweb-4.2.0/cubicweb/server/test_repository/unittest_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/server/utils.py` & `cubicweb-4.2.0/cubicweb/server/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/.gitlab-ci.yml.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/README.rst.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/README.rst.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/__pkginfo__.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/cubicweb_CUBENAME/uiprops.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/setup.py.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/setup.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py` & `cubicweb-4.2.0/cubicweb/skeleton/test/realdb_test_CUBENAME.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/test/test_CUBENAME.py.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/skeleton/tox.ini.tmpl` & `cubicweb-4.2.0/cubicweb/skeleton/tox.ini.tmpl`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py` & `cubicweb-4.2.0/cubicweb/smoke_test/instance_creation_test_cubicweb_api.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py` & `cubicweb-4.2.0/cubicweb/smoke_test/instance_creation_test_cubicweb_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/__init__.py` & `cubicweb-4.2.0/cubicweb/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/ldapparser.py` & `cubicweb-4.2.0/cubicweb/sobjects/ldapparser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/notification.py` & `cubicweb-4.2.0/cubicweb/sobjects/notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/services.py` & `cubicweb-4.2.0/cubicweb/sobjects/services.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/supervising.py` & `cubicweb-4.2.0/cubicweb/sobjects/supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/data/sobjects/__init__.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/data/sobjects/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_email.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/unittest_email.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_notification.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/unittest_notification.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_register_user.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/unittest_register_user.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/sobjects/test/unittest_supervising.py` & `cubicweb-4.2.0/cubicweb/sobjects/test/unittest_supervising.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/tags.py` & `cubicweb-4.2.0/cubicweb/tags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_comment/schema.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_comment/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_email/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_file/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_forge/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_forge/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_mycube/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__init__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/__pkginfo__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_required_variables/site_cubicweb.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/cubicweb_tag/schema.py` & `cubicweb-4.2.0/cubicweb/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/entities.py` & `cubicweb-4.2.0/cubicweb/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/erqlexpr_on_ertype.py` & `cubicweb-4.2.0/cubicweb/test/data/erqlexpr_on_ertype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.0.3_Any.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.0.3_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.0.4_Any.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.0.4_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_Any.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_common.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_common.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.0_repository.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.1.0_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/migration/0.1.2_Any.py` & `cubicweb-4.2.0/cubicweb/test/data/migration/0.1.2_Any.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/rqlexpr_on_ertype_read.py` & `cubicweb-4.2.0/cubicweb/test/data/rqlexpr_on_ertype_read.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_attr.py` & `cubicweb-4.2.0/cubicweb/test/data/rrqlexpr_on_attr.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/rrqlexpr_on_eetype.py` & `cubicweb-4.2.0/cubicweb/test/data/rrqlexpr_on_eetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/schema.py` & `cubicweb-4.2.0/cubicweb/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py` & `cubicweb-4.2.0/cubicweb/test/data/server_migration/bootstrapmigration_repository.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py` & `cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py` & `cubicweb-4.2.0/cubicweb/test/data-rewrite/cubicweb_localperms/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data-rewrite/schema.py` & `cubicweb-4.2.0/cubicweb/test/data-rewrite/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/data_schemareader/schema.py` & `cubicweb-4.2.0/cubicweb/test/data_schemareader/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_binary.py` & `cubicweb-4.2.0/cubicweb/test/unittest_binary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_cwconfig.py` & `cubicweb-4.2.0/cubicweb/test/unittest_cwconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_cwctl.py` & `cubicweb-4.2.0/cubicweb/test/unittest_cwctl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_entity.py` & `cubicweb-4.2.0/cubicweb/test/unittest_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_fast_drop_entities.py` & `cubicweb-4.2.0/cubicweb/test/unittest_fast_drop_entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_mail.py` & `cubicweb-4.2.0/cubicweb/test/unittest_mail.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_migration.py` & `cubicweb-4.2.0/cubicweb/test/unittest_migration.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_predicates.py` & `cubicweb-4.2.0/cubicweb/test/unittest_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_repoapi.py` & `cubicweb-4.2.0/cubicweb/test/unittest_repoapi.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_req.py` & `cubicweb-4.2.0/cubicweb/test/unittest_req.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_rqlrewrite.py` & `cubicweb-4.2.0/cubicweb/test/unittest_rqlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_rqlsuggestions.py` & `cubicweb-4.2.0/cubicweb/test/unittest_rqlsuggestions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_rset.py` & `cubicweb-4.2.0/cubicweb/test/unittest_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_rtags.py` & `cubicweb-4.2.0/cubicweb/test/unittest_rtags.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_schema.py` & `cubicweb-4.2.0/cubicweb/test/unittest_schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_toolsutils.py` & `cubicweb-4.2.0/cubicweb/test/unittest_toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_uilib.py` & `cubicweb-4.2.0/cubicweb/test/unittest_uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_vregistry.py` & `cubicweb-4.2.0/cubicweb/test/unittest_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/test/unittest_wfutils.py` & `cubicweb-4.2.0/cubicweb/test/unittest_wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/toolsutils.py` & `cubicweb-4.2.0/cubicweb/toolsutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/transaction.py` & `cubicweb-4.2.0/cubicweb/transaction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/uilib.py` & `cubicweb-4.2.0/cubicweb/uilib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/utils.py` & `cubicweb-4.2.0/cubicweb/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/wfutils.py` & `cubicweb-4.2.0/cubicweb/wfutils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb/xy.py` & `cubicweb-4.2.0/cubicweb/xy.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/cubicweb.egg-info/PKG-INFO` & `cubicweb-4.2.0/cubicweb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb
-Version: 4.1.0
+Version: 4.2.0
 Summary: a repository of entities / relations for knowledge management
 Home-page: https://www.cubicweb.org
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Requires-Python: >=3.7
 Provides-Extra: captcha
```

### Comparing `cubicweb-4.1.0/cubicweb.egg-info/SOURCES.txt` & `cubicweb-4.2.0/cubicweb.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -170,14 +170,15 @@
 cubicweb/pyramid/__init__.py
 cubicweb/pyramid/auth.py
 cubicweb/pyramid/config.py
 cubicweb/pyramid/core.py
 cubicweb/pyramid/csrf.py
 cubicweb/pyramid/debug_source_code.py
 cubicweb/pyramid/debugtoolbar_panels.py
+cubicweb/pyramid/default_session.py
 cubicweb/pyramid/development.ini.tmpl
 cubicweb/pyramid/predicates.py
 cubicweb/pyramid/pyramid.ini.tmpl
 cubicweb/pyramid/pyramidctl.py
 cubicweb/pyramid/resources.py
 cubicweb/pyramid/rest_api.py
 cubicweb/pyramid/session.py
@@ -926,14 +927,15 @@
 doc/changes/3.34.rst
 doc/changes/3.35.rst
 doc/changes/3.36.rst
 doc/changes/3.37.rst
 doc/changes/3.38.rst
 doc/changes/4.0.rst
 doc/changes/4.1.rst
+doc/changes/4.2.rst
 doc/changes/changelog.rst
 doc/changes/index.rst
 doc/dev/coding_standards_css.rst
 doc/dev/coding_standards_js.rst
 doc/dev/continuous-integration.rst
 doc/dev/documenting.txt
 doc/dev/features_list.rst
```

### Comparing `cubicweb-4.1.0/doc/4.0.0_how_to_migrate.rst` & `cubicweb-4.2.0/doc/4.0.0_how_to_migrate.rst`

 * *Files 4% similar despite different names*

```diff
@@ -36,23 +36,24 @@
 - All methods, attributes and properties related to CubicWeb-Web in :code:`cubicweb.devtools.testlib.CubicWebTC`
   class have been moved into the class :code:`cubicweb_web.devtools.testlib.WebCWTC`,
   which is now the base class for all CubicWeb-Web related tests (if you need
   Pyramid and CubicWeb-Web, you'll have to use :code:`cubicweb_web.devtools.testlib.PyramidWebCWTC`).
 - :code:`cubicweb.devtools.fake.FakeRequest` have been moved to
   :code:`cubicweb_web.devtools.testlib`.
 - :code:`cubicweb.ext.rest` have been moved to :code:`cubicweb_web.ext.rest`, thus
-  :code:`cubicweb.devtools.apptest_config.ApptestConfiguration` no llonger initialize rest components.
+  :code:`cubicweb.devtools.apptest_config.ApptestConfiguration` no longer initialize rest components.
 - :code:`cubicweb.predicates.paginated_rset` have been moved to :code:`cubicweb_web.predicates.paginated_rset`.
 - :code:`cubicweb.pyramid.url_redirections` have been moved to :code:`cubicweb_web.pyramid.url_redirection`,
   thus, :code:`add_redirection_rule` pyramid directive is no longer usable without :code:`cubicweb_web`.
 - :code:`cubicweb.utils.HTMLHead` and :code:`cubicweb.utils.HTMLStream` have been
   moved to :code:`cubicweb_web.utils`.
 - :code:`has_cw_permission` pyramid view and route predicates are now in :code:`cubicweb_web.pyramid.predicates`
 - :code:`cubicweb.rset.limited_rql` :code:`ResultSet` method is now a function which can be called from
-  :code:`cubicweb_web.views.navigation.limited_rql`.
+  :code:`cubicweb_web.views.navigation.limited_rql` and :code:`_limit_offset_rql` :code:`ResultSet` method
+  is now a function which can be called from :code:`cubicweb_web.views.navigation._limit_offset_rql`.
 - :code:`cubicweb.web.webconfig.WebConfiguration` have been moved to :code:`cubicweb_web.webconfig`.
 - :code:`cubicweb.devtools.RealDatabaseConfiguration` have been removed. You can redo
   it yourself by heriting from :code:`cubicweb.devtools.apptest_config.ApptestConfiguration`
   and adding the following class attributes: :code:`skip_db_create_and_restore = True`
   and :code:`read_instance_schema = True`.
 - by default, there is no more session added to the pyramid request. Thus,
   you cannot access :code:`request.session` anymore if you don't use
```

### Comparing `cubicweb-4.1.0/doc/Makefile` & `cubicweb-4.2.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/_static/favicon.ico` & `cubicweb-4.2.0/doc/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/_static/logo-cubicweb.svg` & `cubicweb-4.2.0/doc/_static/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/announce.en.txt` & `cubicweb-4.2.0/doc/announce.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/announce.fr.txt` & `cubicweb-4.2.0/doc/announce.fr.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/api/__init__.rst` & `cubicweb-4.2.0/doc/api/__init__.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/api/cwvreg.rst` & `cubicweb-4.2.0/doc/api/cwvreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/api/predicates.rst` & `cubicweb-4.2.0/doc/api/predicates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/api/urlpublishing.rst` & `cubicweb-4.2.0/doc/api/urlpublishing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/api/web.rst` & `cubicweb-4.2.0/doc/api/web.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-app.en.txt` & `cubicweb-4.2.0/doc/book/MERGE_ME-tut-create-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt` & `cubicweb-4.2.0/doc/book/MERGE_ME-tut-create-gae-app.en.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/_maybe_to_integrate/rss-xml.rst` & `cubicweb-4.2.0/doc/book/_maybe_to_integrate/rss-xml.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/_maybe_to_integrate/template.rst` & `cubicweb-4.2.0/doc/book/_maybe_to_integrate/template.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/additionnal_services/undo.rst` & `cubicweb-4.2.0/doc/book/additionnal_services/undo.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/backups.rst` & `cubicweb-4.2.0/doc/book/admin/backups.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/config.rst` & `cubicweb-4.2.0/doc/book/admin/config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/create-instance.rst` & `cubicweb-4.2.0/doc/book/admin/create-instance.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/cubicweb-ctl.rst` & `cubicweb-4.2.0/doc/book/admin/cubicweb-ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/deploy.rst` & `cubicweb-4.2.0/doc/book/admin/deploy.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/instance-config.rst` & `cubicweb-4.2.0/doc/book/admin/instance-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/ldap.rst` & `cubicweb-4.2.0/doc/book/admin/ldap.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/setup.rst` & `cubicweb-4.2.0/doc/book/admin/setup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/admin/site-config.rst` & `cubicweb-4.2.0/doc/book/admin/site-config.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/depends.rst` & `cubicweb-4.2.0/doc/book/annexes/depends.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/docstrings-conventions.rst` & `cubicweb-4.2.0/doc/book/annexes/docstrings-conventions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/faq.rst` & `cubicweb-4.2.0/doc/book/annexes/faq.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/mercurial.rst` & `cubicweb-4.2.0/doc/book/annexes/mercurial.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/Graph-ex.gif` & `cubicweb-4.2.0/doc/book/annexes/rql/Graph-ex.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/debugging.rst` & `cubicweb-4.2.0/doc/book/annexes/rql/debugging.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/implementation.rst` & `cubicweb-4.2.0/doc/book/annexes/rql/implementation.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/intro.rst` & `cubicweb-4.2.0/doc/book/annexes/rql/intro.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/language.rst` & `cubicweb-4.2.0/doc/book/annexes/rql/language.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/annexes/rql/usecases.rst` & `cubicweb-4.2.0/doc/book/annexes/rql/usecases.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/connections_pooler.rst` & `cubicweb-4.2.0/doc/book/devrepo/connections_pooler.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/cubes/available-cubes.rst` & `cubicweb-4.2.0/doc/book/devrepo/cubes/available-cubes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/cubes/cc-newcube.rst` & `cubicweb-4.2.0/doc/book/devrepo/cubes/cc-newcube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/cubes/layout.rst` & `cubicweb-4.2.0/doc/book/devrepo/cubes/layout.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/cubes/what-is-a-cube.rst` & `cubicweb-4.2.0/doc/book/devrepo/cubes/what-is-a-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/dataimport.rst` & `cubicweb-4.2.0/doc/book/devrepo/dataimport.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/datamodel/baseschema.rst` & `cubicweb-4.2.0/doc/book/devrepo/datamodel/baseschema.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/datamodel/define-workflows.rst` & `cubicweb-4.2.0/doc/book/devrepo/datamodel/define-workflows.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/datamodel/definition.rst` & `cubicweb-4.2.0/doc/book/devrepo/datamodel/definition.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/datamodel/metadata.rst` & `cubicweb-4.2.0/doc/book/devrepo/datamodel/metadata.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/debug_channels.rst` & `cubicweb-4.2.0/doc/book/devrepo/debug_channels.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/devcore/reqbase.rst` & `cubicweb-4.2.0/doc/book/devrepo/devcore/reqbase.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/entityclasses/adapters.rst` & `cubicweb-4.2.0/doc/book/devrepo/entityclasses/adapters.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/entityclasses/application-logic.rst` & `cubicweb-4.2.0/doc/book/devrepo/entityclasses/application-logic.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/entityclasses/data-as-objects.rst` & `cubicweb-4.2.0/doc/book/devrepo/entityclasses/data-as-objects.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/entityclasses/load-sort.rst` & `cubicweb-4.2.0/doc/book/devrepo/entityclasses/load-sort.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/fti.rst` & `cubicweb-4.2.0/doc/book/devrepo/fti.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/migration.rst` & `cubicweb-4.2.0/doc/book/devrepo/migration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/profiling.rst` & `cubicweb-4.2.0/doc/book/devrepo/profiling.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/repo/hooks.rst` & `cubicweb-4.2.0/doc/book/devrepo/repo/hooks.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/repo/notifications.rst` & `cubicweb-4.2.0/doc/book/devrepo/repo/notifications.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/repo/sessions.rst` & `cubicweb-4.2.0/doc/book/devrepo/repo/sessions.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/testing.rst` & `cubicweb-4.2.0/doc/book/devrepo/testing.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devrepo/vreg.rst` & `cubicweb-4.2.0/doc/book/devrepo/vreg.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/ajax.rst` & `cubicweb-4.2.0/doc/book/devweb/ajax.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/controllers.rst` & `cubicweb-4.2.0/doc/book/devweb/controllers.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/css.rst` & `cubicweb-4.2.0/doc/book/devweb/css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/edition/dissection.rst` & `cubicweb-4.2.0/doc/book/devweb/edition/dissection.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/edition/editcontroller.rst` & `cubicweb-4.2.0/doc/book/devweb/edition/editcontroller.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/edition/examples.rst` & `cubicweb-4.2.0/doc/book/devweb/edition/examples.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/edition/form.rst` & `cubicweb-4.2.0/doc/book/devweb/edition/form.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/facets.rst` & `cubicweb-4.2.0/doc/book/devweb/facets.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/httpcaching.rst` & `cubicweb-4.2.0/doc/book/devweb/httpcaching.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/internationalization.rst` & `cubicweb-4.2.0/doc/book/devweb/internationalization.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/js.rst` & `cubicweb-4.2.0/doc/book/devweb/js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/publisher.rst` & `cubicweb-4.2.0/doc/book/devweb/publisher.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/request.rst` & `cubicweb-4.2.0/doc/book/devweb/request.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/resource.rst` & `cubicweb-4.2.0/doc/book/devweb/resource.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/searchbar.rst` & `cubicweb-4.2.0/doc/book/devweb/searchbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/basetemplates.rst` & `cubicweb-4.2.0/doc/book/devweb/views/basetemplates.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/baseviews.rst` & `cubicweb-4.2.0/doc/book/devweb/views/baseviews.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/boxes.rst` & `cubicweb-4.2.0/doc/book/devweb/views/boxes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/breadcrumbs.rst` & `cubicweb-4.2.0/doc/book/devweb/views/breadcrumbs.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/idownloadable.rst` & `cubicweb-4.2.0/doc/book/devweb/views/idownloadable.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/primary.rst` & `cubicweb-4.2.0/doc/book/devweb/views/primary.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/reledit.rst` & `cubicweb-4.2.0/doc/book/devweb/views/reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/startup.rst` & `cubicweb-4.2.0/doc/book/devweb/views/startup.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/table.rst` & `cubicweb-4.2.0/doc/book/devweb/views/table.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/urlpublish.rst` & `cubicweb-4.2.0/doc/book/devweb/views/urlpublish.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/views.rst` & `cubicweb-4.2.0/doc/book/devweb/views/views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/views/xmlrss.rst` & `cubicweb-4.2.0/doc/book/devweb/views/xmlrss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/devweb/warning.rst` & `cubicweb-4.2.0/doc/book/devweb/warning.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/intro/concepts.rst` & `cubicweb-4.2.0/doc/book/intro/concepts.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/intro/history.rst` & `cubicweb-4.2.0/doc/book/intro/history.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/auth.rst` & `cubicweb-4.2.0/doc/book/pyramid/auth.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/ctl.rst` & `cubicweb-4.2.0/doc/book/pyramid/ctl.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/debug_toolbar.rst` & `cubicweb-4.2.0/doc/book/pyramid/debug_toolbar.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/index.rst` & `cubicweb-4.2.0/doc/book/pyramid/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/quickstart.rst` & `cubicweb-4.2.0/doc/book/pyramid/quickstart.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/pyramid/settings.rst` & `cubicweb-4.2.0/doc/book/pyramid/settings.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/security/csrf.rst` & `cubicweb-4.2.0/doc/book/security/csrf.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/src/archi_globale.dia` & `cubicweb-4.2.0/doc/book/src/archi_globale.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/book/src/main_template_layout.dia` & `cubicweb-4.2.0/doc/book/src/main_template_layout.dia`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.14.rst` & `cubicweb-4.2.0/doc/changes/3.14.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.15.rst` & `cubicweb-4.2.0/doc/changes/3.15.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.16.rst` & `cubicweb-4.2.0/doc/changes/3.16.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.17.rst` & `cubicweb-4.2.0/doc/changes/3.17.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.18.rst` & `cubicweb-4.2.0/doc/changes/3.18.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.19.rst` & `cubicweb-4.2.0/doc/changes/3.19.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.20.rst` & `cubicweb-4.2.0/doc/changes/3.20.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.21.rst` & `cubicweb-4.2.0/doc/changes/3.21.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.22.rst` & `cubicweb-4.2.0/doc/changes/3.22.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.23.rst` & `cubicweb-4.2.0/doc/changes/3.23.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.24.rst` & `cubicweb-4.2.0/doc/changes/3.24.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.25.rst` & `cubicweb-4.2.0/doc/changes/3.25.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.27.rst` & `cubicweb-4.2.0/doc/changes/3.27.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.28.rst` & `cubicweb-4.2.0/doc/changes/3.28.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.29.rst` & `cubicweb-4.2.0/doc/changes/3.29.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.30.rst` & `cubicweb-4.2.0/doc/changes/3.30.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.31.rst` & `cubicweb-4.2.0/doc/changes/3.31.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.32.rst` & `cubicweb-4.2.0/doc/changes/3.32.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.32_reledit.rst` & `cubicweb-4.2.0/doc/changes/3.32_reledit.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.33.rst` & `cubicweb-4.2.0/doc/changes/3.33.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.34.rst` & `cubicweb-4.2.0/doc/changes/3.34.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.35.rst` & `cubicweb-4.2.0/doc/changes/3.35.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.36.rst` & `cubicweb-4.2.0/doc/changes/3.36.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/3.37.rst` & `cubicweb-4.2.0/doc/changes/3.37.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.37.17 (2023-07-10)
+====================
+👷 Bug fixes
+-----------
+
+- migration: allow to drop a cube even if it's a dependency (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/774)
+
 3.37.16 (2023-06-07)
 ====================
 👷 Bug fixes
 -----------
 
 - pyramid: allows to use None for timeout, max_age and reissue_time options
```

### Comparing `cubicweb-4.1.0/doc/changes/3.38.rst` & `cubicweb-4.2.0/doc/changes/3.38.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+3.38.10 (2023-07-10)
+====================
+👷 Bug fixes
+-----------
+
+- migration: allow to drop a cube even if it's a dependency (https://forge.extranet.logilab.fr/cubicweb/cubicweb/-/issues/774)
+
 3.38.9 (2023-06-07)
 ===================
 👷 Bug fixes
 -----------
 
 - pyramid: allows to use None for timeout, max_age and reissue_time options
```

### Comparing `cubicweb-4.1.0/doc/changes/4.0.rst` & `cubicweb-4.2.0/doc/changes/4.0.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/4.1.rst` & `cubicweb-4.2.0/doc/changes/4.1.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/changes/changelog.rst` & `cubicweb-4.2.0/doc/changes/changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 .. -*- coding: utf-8 -*-
 
+.. include:: 4.2.rst
 .. include:: 4.1.rst
 .. include:: 4.0.rst
 
 .. include:: 3.38.rst
 .. include:: 3.37.rst
 .. include:: 3.36.rst
```

### Comparing `cubicweb-4.1.0/doc/conf.py` & `cubicweb-4.2.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/coding_standards_css.rst` & `cubicweb-4.2.0/doc/dev/coding_standards_css.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/coding_standards_js.rst` & `cubicweb-4.2.0/doc/dev/coding_standards_js.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/continuous-integration.rst` & `cubicweb-4.2.0/doc/dev/continuous-integration.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/documenting.txt` & `cubicweb-4.2.0/doc/dev/documenting.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/features_list.rst` & `cubicweb-4.2.0/doc/dev/features_list.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/install_from_sources.rst` & `cubicweb-4.2.0/doc/dev/install_from_sources.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/dev/refactoring-the-css-with-uiprops.rst` & `cubicweb-4.2.0/doc/dev/refactoring-the-css-with-uiprops.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/03-transitions-view_en.png` & `cubicweb-4.2.0/doc/images/03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/breadcrumbs_header.png` & `cubicweb-4.2.0/doc/images/breadcrumbs_header.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_general_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_general_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_registry_content_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_registry_content_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_registry_decisions_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_registry_decisions_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_rql_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_rql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_rql_traceback_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_rql_traceback_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_show_source.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_show_source.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_show_source_link.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_show_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_sql_panel.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_sql_panel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/debugtoolbar_traceback_source_link.png` & `cubicweb-4.2.0/doc/images/debugtoolbar_traceback_source_link.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/example-card-with-rql-directive.png` & `cubicweb-4.2.0/doc/images/example-card-with-rql-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/example-card-with-rql-table-directive.png` & `cubicweb-4.2.0/doc/images/example-card-with-rql-table-directive.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/facet_date_range.png` & `cubicweb-4.2.0/doc/images/facet_date_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/facet_has_image.png` & `cubicweb-4.2.0/doc/images/facet_has_image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/facet_overview.png` & `cubicweb-4.2.0/doc/images/facet_overview.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/facet_range.png` & `cubicweb-4.2.0/doc/images/facet_range.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_00-login_en.png` & `cubicweb-4.2.0/doc/images/lax-book_00-login_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_01-start_en.png` & `cubicweb-4.2.0/doc/images/lax-book_01-start_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_02-cookie-values_en.png` & `cubicweb-4.2.0/doc/images/lax-book_02-cookie-values_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_02-create-blog_en.png` & `cubicweb-4.2.0/doc/images/lax-book_02-create-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_03-list-one-blog_en.png` & `cubicweb-4.2.0/doc/images/lax-book_03-list-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_03-site-config-panel_en.png` & `cubicweb-4.2.0/doc/images/lax-book_03-site-config-panel_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_03-state-submitted_en.png` & `cubicweb-4.2.0/doc/images/lax-book_03-state-submitted_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_03-transitions-view_en.png` & `cubicweb-4.2.0/doc/images/lax-book_03-transitions-view_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_04-detail-one-blog_en.png` & `cubicweb-4.2.0/doc/images/lax-book_04-detail-one-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_05-list-two-blog_en.png` & `cubicweb-4.2.0/doc/images/lax-book_05-list-two-blog_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_06-add-relation-entryof_en.png` & `cubicweb-4.2.0/doc/images/lax-book_06-add-relation-entryof_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_06-main-template-logo_en.png` & `cubicweb-4.2.0/doc/images/lax-book_06-main-template-logo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_07-detail-one-blogentry_en.png` & `cubicweb-4.2.0/doc/images/lax-book_07-detail-one-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_08-schema_en.png` & `cubicweb-4.2.0/doc/images/lax-book_08-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_09-new-view-blogentry_en.png` & `cubicweb-4.2.0/doc/images/lax-book_09-new-view-blogentry_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/lax-book_10-blog-with-two-entries_en.png` & `cubicweb-4.2.0/doc/images/lax-book_10-blog-with-two-entries_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/main_template.png` & `cubicweb-4.2.0/doc/images/main_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/main_template.svg` & `cubicweb-4.2.0/doc/images/main_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/main_template_layout.png` & `cubicweb-4.2.0/doc/images/main_template_layout.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/primaryview_template.png` & `cubicweb-4.2.0/doc/images/primaryview_template.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/primaryview_template.svg` & `cubicweb-4.2.0/doc/images/primaryview_template.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/request_session.png` & `cubicweb-4.2.0/doc/images/request_session.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/request_session.svg` & `cubicweb-4.2.0/doc/images/request_session.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/server-class-diagram.png` & `cubicweb-4.2.0/doc/images/server-class-diagram.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_blog-form_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_blog-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_blog-primary-after-post-creation_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_blog-primary_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_blog-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_blogs-list_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_blogs-list_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_form-generic-relations_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_form-generic-relations_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_index_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_index_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_index_gettext_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_index_gettext_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_index_logged_in_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_index_logged_in_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_login-form_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_login-form_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-blogentry-taggable-commentable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-custom-primary_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-community-custom-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-default-primary_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-community-default-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-community-taggable-primary_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-custom-footer_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-custom-footer_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-schema_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_myblog-siteinfo_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_myblog-siteinfo_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_schema_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_schema_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_schema_graphviz_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_schema_graphviz_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-base_siteconfig_en.png` & `cubicweb-4.2.0/doc/images/tutos-base_siteconfig_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_admin.png` & `cubicweb-4.2.0/doc/images/tutos-museum_admin.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_city_created.png` & `cubicweb-4.2.0/doc/images/tutos-museum_city_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_city_creation.png` & `cubicweb-4.2.0/doc/images/tutos-museum_city_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_data_model_schema.png` & `cubicweb-4.2.0/doc/images/tutos-museum_data_model_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_empty_instance.png` & `cubicweb-4.2.0/doc/images/tutos-museum_empty_instance.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_finished_import.png` & `cubicweb-4.2.0/doc/images/tutos-museum_finished_import.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_list_view.png` & `cubicweb-4.2.0/doc/images/tutos-museum_list_view.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_museum_created.png` & `cubicweb-4.2.0/doc/images/tutos-museum_museum_created.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_museum_creation.png` & `cubicweb-4.2.0/doc/images/tutos-museum_museum_creation.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_museum_with_city_name.png` & `cubicweb-4.2.0/doc/images/tutos-museum_museum_with_city_name.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_react_map.png` & `cubicweb-4.2.0/doc/images/tutos-museum_react_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-museum_with_schema.png` & `cubicweb-4.2.0/doc/images/tutos-museum_with_schema.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_background-image.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_background-image.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_boxes.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_boxes.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_breadcrumbs.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_breadcrumbs.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_facets.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_facets.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_grey-box.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_grey-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_index-after.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_index-after.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_index-before.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_index-before.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_login-box.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_login-box.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_prevnext.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_prevnext.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui1.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_ui1.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui2.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_ui2.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/tutos-photowebsite_ui3.png` & `cubicweb-4.2.0/doc/images/tutos-photowebsite_ui3.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/undo_history-view_w600.png` & `cubicweb-4.2.0/doc/images/undo_history-view_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/undo_mesage_w600.png` & `cubicweb-4.2.0/doc/images/undo_mesage_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/undo_startup-link_w600.png` & `cubicweb-4.2.0/doc/images/undo_startup-link_w600.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/views-table-filter-shadow.png` & `cubicweb-4.2.0/doc/images/views-table-filter-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/views-table-filter.png` & `cubicweb-4.2.0/doc/images/views-table-filter.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/views-table-shadow.png` & `cubicweb-4.2.0/doc/images/views-table-shadow.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/images/views-table.png` & `cubicweb-4.2.0/doc/images/views-table.png`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/index.rst` & `cubicweb-4.2.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/plan_formation_python_cubicweb.txt` & `cubicweb-4.2.0/doc/plan_formation_python_cubicweb.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tools/generate_modules.py` & `cubicweb-4.2.0/doc/tools/generate_modules.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tools/mode_plan.py` & `cubicweb-4.2.0/doc/tools/mode_plan.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tools/pyjsrest.py` & `cubicweb-4.2.0/doc/tools/pyjsrest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/index.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/part01_create-cube.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/part01_create-cube.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/part02_security.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/part02_security.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/part03_bfss.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/part03_bfss.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/part04_ui-base.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/part04_ui-base.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/advanced/part05_ui-advanced.rst` & `cubicweb-4.2.0/doc/tutorials/advanced/part05_ui-advanced.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/base/blog-in-five-minutes.rst` & `cubicweb-4.2.0/doc/tutorials/base/blog-in-five-minutes.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/base/conclusion.rst` & `cubicweb-4.2.0/doc/tutorials/base/conclusion.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/base/customizing-the-application.rst` & `cubicweb-4.2.0/doc/tutorials/base/customizing-the-application.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/base/discovering-the-ui.rst` & `cubicweb-4.2.0/doc/tutorials/base/discovering-the-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/base/index.rst` & `cubicweb-4.2.0/doc/tutorials/base/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_import.py` & `cubicweb-4.2.0/doc/tutorials/dataimport/diseasome_import.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/dataimport/diseasome_parser.py` & `cubicweb-4.2.0/doc/tutorials/dataimport/diseasome_parser.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/dataimport/index.rst` & `cubicweb-4.2.0/doc/tutorials/dataimport/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/dataimport/schema.py` & `cubicweb-4.2.0/doc/tutorials/dataimport/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/index.rst` & `cubicweb-4.2.0/doc/tutorials/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/data-management.rst` & `cubicweb-4.2.0/doc/tutorials/museum/data-management.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/develop-app.rst` & `cubicweb-4.2.0/doc/tutorials/museum/develop-app.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/develop-ui.rst` & `cubicweb-4.2.0/doc/tutorials/museum/develop-ui.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/enhance-views.rst` & `cubicweb-4.2.0/doc/tutorials/museum/enhance-views.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/getting-started.rst` & `cubicweb-4.2.0/doc/tutorials/museum/getting-started.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/doc/tutorials/museum/index.rst` & `cubicweb-4.2.0/doc/tutorials/museum/index.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/extras/cubicweb-ctl.bash_completion` & `cubicweb-4.2.0/extras/cubicweb-ctl.bash_completion`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/jshintrc` & `cubicweb-4.2.0/jshintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/man/cubicweb-ctl.1` & `cubicweb-4.2.0/man/cubicweb-ctl.1`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/pylintrc` & `cubicweb-4.2.0/pylintrc`

 * *Files identical despite different names*

### Comparing `cubicweb-4.1.0/setup.py` & `cubicweb-4.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     packages=find_packages(),
     package_data=package_data,
     include_package_data=True,
     install_requires=[
         "logilab-common >= 1.8.3, < 2.0.0",
         "logilab-mtconverter >= 0.9.2, < 1.0.0",
         "rql >= 0.39, < 1.0.0",
-        "yams >= 0.49.0, < 0.50.0",
+        "yams >= 0.50.0, < 1.0.0",
         "lxml",
         "logilab-database >= 1.18.2, < 2.0.0",
         "passlib >= 1.7",
         "pytz",
         "Markdown >= 3.4.0",
         "filelock",
         "rdflib >= 6.0.0",
```

### Comparing `cubicweb-4.1.0/tox.ini` & `cubicweb-4.2.0/tox.ini`

 * *Files identical despite different names*

