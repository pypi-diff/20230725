# Comparing `tmp/acs-axiom-0.1.4.tar.gz` & `tmp/acs-axiom-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acs-axiom-0.1.4.tar", last modified: Sat Apr 29 12:38:11 2023, max compression
+gzip compressed data, was "acs-axiom-0.1.5.tar", last modified: Tue Jul 25 10:23:44 2023, max compression
```

## Comparing `acs-axiom-0.1.4.tar` & `acs-axiom-0.1.5.tar`

### file list

```diff
@@ -1,241 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.693480 acs-axiom-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.629476 acs-axiom-0.1.4/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.github/issue-branch.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.629476 acs-axiom-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.github/workflows/create-issue-branch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.github/workflows/python-package-conda.yml
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 12:38:11.693480 acs-axiom-0.1.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.629476 acs-axiom-0.1.4/acs_axiom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 12:38:11.000000 acs-axiom-0.1.4/acs_axiom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.633476 acs-axiom-0.1.4/axiom/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/ccam_test.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/converters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.633476 acs-axiom-0.1.4/axiom/data/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/domains.json
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/drs.json
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/models.json
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/projects.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.641477 acs-axiom-0.1.4/axiom/data/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)  6871846 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cf-77.json
--rw-r--r--   0 runner    (1001) docker     (123)   104156 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cordex-cmip6.json
--rw-r--r--   0 runner    (1001) docker     (123)    72349 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cordex-day.json
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cordex-fx.json
--rw-r--r--   0 runner    (1001) docker     (123)   118873 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cordex-month.json
--rw-r--r--   0 runner    (1001) docker     (123)   104150 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/cordex.json
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/data/schemas/mrd-0.1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.641477 acs-axiom-0.1.4/axiom/drs/
--rw-r--r--   0 runner    (1001) docker     (123)    26001 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/payload.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.641477 acs-axiom-0.1.4/axiom/drs/processing/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/processing/ccam.py
--rw-r--r--   0 runner    (1001) docker     (123)    15882 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/drs.old.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.641477 acs-axiom-0.1.4/axiom/qa/
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/qa/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.641477 acs-axiom-0.1.4/axiom/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/schemas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/axiom/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/axiom/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/data/mrd.xml
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_drs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_drs_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_payloads.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/tests/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/axiom/validation/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/axiom/validation/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/bin/axiom
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.629476 acs-axiom-0.1.4/docs/build/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/docs/build/doctrees/
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/cli.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/conversion.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    25138 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/environment.pickle
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/index.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/installation.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/metadata.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     7552 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/reporting.doctree
--rw-r--r--   0 runner    (1001) docker     (123)    12008 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/schemas.doctree
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/doctrees/validation.doctree
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.645477 acs-axiom-0.1.4/docs/build/html/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/.buildinfo
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.649477 acs-axiom-0.1.4/docs/build/html/_modules/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.649477 acs-axiom-0.1.4/docs/build/html/_modules/axiom/
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_modules/axiom/parsers.html
--rw-r--r--   0 runner    (1001) docker     (123)    12516 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_modules/axiom.html
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_modules/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.649477 acs-axiom-0.1.4/docs/build/html/_sources/
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/cli.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/conversion.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/index.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/installation.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/metadata.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/reporting.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/schemas.rst.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_sources/validation.rst.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.653478 acs-axiom-0.1.4/docs/build/html/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    11185 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/alabaster.css
--rw-r--r--   0 runner    (1001) docker     (123)    14652 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/basic.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.653478 acs-axiom-0.1.4/docs/build/html/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/badge_only.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.657478 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-normal.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/fonts/lato-normal.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   123687 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/css/theme.css
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/doctools.js
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/documentation_options.js
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/file.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.665478 acs-axiom-0.1.4/docs/build/html/_static/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)   109948 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Inconsolata-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    96964 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Inconsolata-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63184 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Inconsolata.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.673479 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/
--rw-r--r--   0 runner    (1001) docker     (123)   256056 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   600856 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   309728 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)   184912 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   266158 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bolditalic.eot
--rw-r--r--   0 runner    (1001) docker     (123)   622572 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bolditalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   323344 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   193308 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-bolditalic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   268604 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-italic.eot
--rw-r--r--   0 runner    (1001) docker     (123)   639388 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   328412 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-italic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   195704 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-italic.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   253461 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   607720 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   309192 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)   182708 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato/lato-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   656544 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   656568 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/Lato-Regular.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.677479 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/
--rw-r--r--   0 runner    (1001) docker     (123)    79520 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.eot
--rw-r--r--   0 runner    (1001) docker     (123)   170616 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    87624 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff
--rw-r--r--   0 runner    (1001) docker     (123)    67312 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-bold.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    78331 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)   169064 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    86288 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff
--rw-r--r--   0 runner    (1001) docker     (123)    66444 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab/roboto-slab-v7-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   170616 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   169064 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/RobotoSlab-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   165742 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   444379 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   165548 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    98024 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    77160 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/fonts/fontawesome-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   287630 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    89476 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.677479 acs-axiom-0.1.4/docs/build/html/_static/js/
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/js/badge_only.js
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/js/html5shiv-printshiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/js/html5shiv.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    15414 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/js/modernizr.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/js/theme.js
--rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/language_data.js
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/minus.png
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/plus.png
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)    16578 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/searchtools.js
--rw-r--r--   0 runner    (1001) docker     (123)    67692 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/underscore-1.12.0.js
--rw-r--r--   0 runner    (1001) docker     (123)    68420 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/underscore-1.13.1.js
--rw-r--r--   0 runner    (1001) docker     (123)    19358 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/_static/underscore.js
--rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/cli.html
--rw-r--r--   0 runner    (1001) docker     (123)     9814 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/conversion.html
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/genindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/installation.html
--rw-r--r--   0 runner    (1001) docker     (123)    10345 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/metadata.html
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/objects.inv
--rw-r--r--   0 runner    (1001) docker     (123)     5135 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/py-modindex.html
--rw-r--r--   0 runner    (1001) docker     (123)     7452 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/reporting.html
--rw-r--r--   0 runner    (1001) docker     (123)    11835 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/schemas.html
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     5282 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/searchindex.js
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/build/html/validation.html
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.681479 acs-axiom-0.1.4/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/about.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/axiom.drs.processing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/axiom.drs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/axiom.rst
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/axiom.validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/conversion.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/custom_processors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/drs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/drs_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/payloads.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/performance.rst
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/reporting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/schemas.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/docs/source/validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-29 12:38:11.693480 acs-axiom-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 12:38:11.693480 acs-axiom-0.1.4/specifications/
--rw-r--r--   0 runner    (1001) docker     (123)  6871846 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cf-77.json
--rw-r--r--   0 runner    (1001) docker     (123)  3999936 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)    72025 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex-day.json
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex-fx.json
--rw-r--r--   0 runner    (1001) docker     (123)   118549 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex-month.json
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex_var_info_day.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex_var_info_fx.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/cordex_var_info_mon.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/mrd-0.1.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/mrd-0.2.0.json
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-29 12:37:49.000000 acs-axiom-0.1.4/specifications/mrd.xsd
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.816563 acs-axiom-0.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.768563 acs-axiom-0.1.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.github/issue-branch.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.772563 acs-axiom-0.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.github/workflows/create-issue-branch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.github/workflows/python-package-conda.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-25 10:23:44.816563 acs-axiom-0.1.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.772563 acs-axiom-0.1.5/acs_axiom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2688 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-25 10:23:44.000000 acs-axiom-0.1.5/acs_axiom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.772563 acs-axiom-0.1.5/axiom/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.776563 acs-axiom-0.1.5/axiom/automation/
+-rw-r--r--   0 runner    (1001) docker     (123)     8625 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/automation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/ccam_test.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/converters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.776563 acs-axiom-0.1.5/axiom/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/domains.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/drs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/models.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/projects.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.788563 acs-axiom-0.1.5/axiom/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)  6871846 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cf-77.json
+-rw-r--r--   0 runner    (1001) docker     (123)   104156 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cordex-cmip6.json
+-rw-r--r--   0 runner    (1001) docker     (123)    72349 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cordex-day.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cordex-fx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   118873 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cordex-month.json
+-rw-r--r--   0 runner    (1001) docker     (123)   104150 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/cordex.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/data/schemas/mrd-0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.788563 acs-axiom-0.1.5/axiom/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)    26127 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13845 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/payload.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.788563 acs-axiom-0.1.5/axiom/drs/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/processing/ccam.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21265 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/drs.old.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.788563 acs-axiom-0.1.5/axiom/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13172 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/qa/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.788563 acs-axiom-0.1.5/axiom/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/supervisor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.792563 acs-axiom-0.1.5/axiom/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.792563 acs-axiom-0.1.5/axiom/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/data/mrd.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_drs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_drs_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_payloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/tests/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.792563 acs-axiom-0.1.5/axiom/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/axiom/validation/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.792563 acs-axiom-0.1.5/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/bin/axiom
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.792563 acs-axiom-0.1.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.796563 acs-axiom-0.1.5/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/about.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/axiom.drs.processing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/axiom.drs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/axiom.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/axiom.validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/conversion.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.796563 acs-axiom-0.1.5/docs/source/drs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/custom_processors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/fault-tolerance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/payloads.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/performance.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/drs/typical-workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/reporting.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.796563 acs-axiom-0.1.5/docs/source/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/schemas/schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    34727 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/docs/source/workflow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-07-25 10:23:44.816563 acs-axiom-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 10:23:44.816563 acs-axiom-0.1.5/specifications/
+-rw-r--r--   0 runner    (1001) docker     (123)  6871846 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cf-77.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3999936 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)    72025 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex-day.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex-fx.json
+-rw-r--r--   0 runner    (1001) docker     (123)   118549 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex-month.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex_var_info_day.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex_var_info_fx.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/cordex_var_info_mon.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/mrd-0.1.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/mrd-0.2.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-25 10:23:01.000000 acs-axiom-0.1.5/specifications/mrd.xsd
```

### Comparing `acs-axiom-0.1.4/.github/workflows/ci.yml` & `acs-axiom-0.1.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/.github/workflows/pypi-release.yml` & `acs-axiom-0.1.5/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/.github/workflows/python-package-conda.yml` & `acs-axiom-0.1.5/.github/workflows/python-package-conda.yml`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/.readthedocs.yaml` & `acs-axiom-0.1.5/.readthedocs.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,8 +22,10 @@
 # If using Sphinx, optionally build your docs in additional formats such as PDF
 # formats:
 #    - pdf
 
 # Optionally declare the Python requirements required to build your docs
 python:
    install:
+   - method: pip
+     path: .
    - requirements: docs/requirements.txt
```

### Comparing `acs-axiom-0.1.4/CITATION.cff` & `acs-axiom-0.1.5/CITATION.cff`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/CONTRIBUTING.md` & `acs-axiom-0.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/LICENSE` & `acs-axiom-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/PKG-INFO` & `acs-axiom-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acs-axiom
-Version: 0.1.4
+Version: 0.1.5
 Summary: A prototype utility for validating/applying metadata templates for scientific data.
 Home-page: https://github.com/AusClimateService/axiom
 Author: Ben Schroeter
 Author-email: ben.schroeter@csiro.au
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `acs-axiom-0.1.4/acs_axiom.egg-info/PKG-INFO` & `acs-axiom-0.1.5/acs_axiom.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acs-axiom
-Version: 0.1.4
+Version: 0.1.5
 Summary: A prototype utility for validating/applying metadata templates for scientific data.
 Home-page: https://github.com/AusClimateService/axiom
 Author: Ben Schroeter
 Author-email: ben.schroeter@csiro.au
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `acs-axiom-0.1.4/axiom/ccam_test.sh` & `acs-axiom-0.1.5/axiom/ccam_test.sh`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/config.py` & `acs-axiom-0.1.5/axiom/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,15 +69,18 @@
             defaults_only (bool, optional): Load only the defaults. Defaults to False.
         """
 
         default_filepath = os.path.join(au.get_installed_data_root(), f'{config_name}.json')
         user_filepath = os.path.join(au.get_user_data_root(), f'{config_name}.json')
         
         # Load any installed defaults, if they exists
-        defaults = json.load(open(default_filepath, 'r'))
+        if os.path.isfile(default_filepath):
+            defaults = json.load(open(default_filepath, 'r'))
+        else:
+            defaults = dict()
 
         if defaults_only:
             self.update(defaults)
             return
 
         # Load the user configuration over the top
         if os.path.isfile(user_filepath):
```

### Comparing `acs-axiom-0.1.4/axiom/converters.py` & `acs-axiom-0.1.5/axiom/converters.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/domains.json` & `acs-axiom-0.1.5/axiom/data/domains.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/drs.json` & `acs-axiom-0.1.5/axiom/data/drs.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9591346153846154%*

 * *Differences: {"'filename_filtering'": "{'variable_regex': '^%(variable)s_'}",*

 * * "'processing_timeout_seconds'": '600'}*

```diff
@@ -66,15 +66,15 @@
             "complevel": 1,
             "dtype": "float32",
             "zlib": true
         }
     },
     "filename_filtering": {
         "variable": true,
-        "variable_regex": "^%(variable)s_*",
+        "variable_regex": "^%(variable)s_",
         "year": true,
         "year_offset": 1
     },
     "frequency_mapping": {
         "12min": "12min",
         "1D": "day",
         "1H": "1hr",
@@ -112,14 +112,15 @@
         "rcm_model": "%(rcm_model)s",
         "rcm_model_cordex": "%(rcm_model_cordex)s",
         "rcm_version_cordex": "%(rcm_version_cordex)s",
         "rcm_version_id": "%(rcm_version_id)s",
         "references": "https://confluence.csiro.au/display/CCAM",
         "tracking_id": "%(uuid)s"
     },
+    "processing_timeout_seconds": 600,
     "recoverable_errors": [
         "AttributeError: 'NoneType' object has no attribute 'lock_acquire'"
     ],
     "reference_time": "1949-12-01 00:00:00",
     "rerun_attempts": 3,
     "rerun_failures": false,
     "rolling_time_averaging": true,
```

### Comparing `acs-axiom-0.1.4/axiom/data/models.json` & `acs-axiom-0.1.5/axiom/data/models.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/projects.json` & `acs-axiom-0.1.5/axiom/data/projects.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cf-77.json` & `acs-axiom-0.1.5/axiom/data/schemas/cf-77.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cordex-cmip6.json` & `acs-axiom-0.1.5/axiom/data/schemas/cordex-cmip6.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cordex-day.json` & `acs-axiom-0.1.5/axiom/data/schemas/cordex-day.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cordex-fx.json` & `acs-axiom-0.1.5/axiom/data/schemas/cordex-fx.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cordex-month.json` & `acs-axiom-0.1.5/axiom/data/schemas/cordex-month.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/cordex.json` & `acs-axiom-0.1.5/axiom/data/schemas/cordex.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/data/schemas/mrd-0.1.0.json` & `acs-axiom-0.1.5/axiom/data/schemas/mrd-0.1.0.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/decorators.py` & `acs-axiom-0.1.5/axiom/decorators.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/drs/__init__.py` & `acs-axiom-0.1.5/axiom/drs/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from distributed import Client, LocalCluster
 from axiom.config import load_config
 from axiom import __version__ as axiom_version
 from axiom.exceptions import NoFilesToProcessException, DRSContextInterpolationException
 import shutil
 from dask.distributed import progress, wait
 import numpy as np
+from axiom.supervisor import Supervisor
 
 
 def consume(json_filepath):
     """Consume a json payload (for message passing)
 
     Args:
         json_filepath (str): Path to the JSON file.
@@ -59,14 +60,17 @@
 
     # Mark consumed by touching another file.
     au.touch(consumed_filepath)
 
     # Unlock
     au.unlock(json_filepath)
 
+    # Explicit exit (#125)
+    sys.exit(0)
+
 
 def process(
     input_files,
     output_directory,
     variable,
     project,
     model,
@@ -278,15 +282,15 @@
     logger.debug('Domain: ' + domain.to_directive())
 
     # Subset the geographical domain
     logger.debug('Subsetting geographical domain.')
     ds = domain.subset_xarray(ds, drop=True)
 
     # TODO: Need to find a less manual way to do this.
-    for year in generate_years_list(start_year, end_year):
+    for year in adu.generate_years_list(start_year, end_year):
 
         logger.info(f'Processing {year}')
 
         # Subset the data into just this year
         if not time_invariant:
             time_slice = slice(f'{year}-01-01', f'{year}-12-31')
             _ds = ds.sel(time=time_slice, drop=True)
@@ -328,16 +332,18 @@
             # Update the cell methods below
             resampling_applied = True
 
         # Start persisting the computation now
         _ds = _ds.persist()
 
         # Monthly data should have the days truncated
-        context['start_date'] = f'{year}0101' if output_frequency[-1] != 'M' else f'{year}01'
-        context['end_date'] = f'{year}1231' if output_frequency[-1] != 'M' else f'{year}12'
+        # context['start_date'] = f'{year}0101' if output_frequency[-1] != 'M' else f'{year}01'
+        # context['end_date'] = f'{year}1231' if output_frequency[-1] != 'M' else f'{year}12'
+
+        context['start_date'], context['end_date'] = adu.get_start_and_end_dates(year, output_frequency)
 
         # Tracking info
         context['creation_date'] = datetime.utcnow()
         context['uuid'] = uuid4()
 
         # Interpolate context
         logger.info('Interpolating context.')
@@ -443,42 +449,31 @@
             raise DRSContextInterpolationException(uninterpolated_keys)
 
         # Create the output directory
         output_dir = os.path.dirname(output_filepath)
         logger.debug(f'Creating {output_dir}')
         os.makedirs(output_dir, exist_ok=True)
 
-        logger.info('Waiting for computations to finish.')
-        progress(_ds)
+        # Supervise this job to ensure that it does in fact complete.
+        with Supervisor(seconds=config.processing_timeout_seconds, error_msg=f'Variable {variable} took too long to complete, moving on.'):
+            logger.info('Waiting for computations to finish.')
+            progress(_ds)
 
         logger.debug(f'Writing {output_filepath}')
         write = _ds.to_netcdf(
             output_filepath,
             format='NETCDF4',
             encoding=encoding,
             unlimited_dims=['time']
         )
 
     elapsed_time = timer.stop()
     logger.info(f'DRS processing task took {elapsed_time} seconds.')
 
 
-def generate_years_list(start_year, end_year):
-    """Generate a list of years (decades) to process.
-
-    Args:
-        start_year (int): Start year.
-        end_year (int): End year.
-
-    Returns:
-        iterator : Years to process.
-    """
-    return range(start_year, end_year+1, 10)
-
-
 def load_variable_config(project_config):
     """Extract the variable configuration out of the project configuration.
 
     Args:
         project_config (dict-like): Project configuration.
 
     Returns:
```

### Comparing `acs-axiom-0.1.4/axiom/drs/cli.py` & `acs-axiom-0.1.5/axiom/drs/cli.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/drs/domain.py` & `acs-axiom-0.1.5/axiom/drs/domain.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/drs/payload.py` & `acs-axiom-0.1.5/axiom/drs/payload.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,23 +93,26 @@
         
         Examples:
             >>> payload = Payload.from_dict(d)
         """
         return Payload(**d)
     
 
-    def to_json(self, filepath):
+    def to_json(self, filepath=None):
         """Serialize the Payload to the filepath (save as JSON).
 
         Args:
-            filepath (str): Filepath.
+            filepath (str, optional): Filepath to write. Defaults to None (Writes default filename to current directory).
         
         Examples:
             >>> payload.to_json('payload.json')
         """
+        if filepath is None:
+            filepath = self.get_filename()
+
         _dict = self.to_dict()
         with open(filepath, 'w') as f:
             f.write(json.dumps(_dict, indent=4))
 
 
     def from_json(filepath):
         """Instantiate a payload from a json filepath.
```

### Comparing `acs-axiom-0.1.4/axiom/drs/processing/ccam.py` & `acs-axiom-0.1.5/axiom/drs/processing/ccam.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/drs/utilities.py` & `acs-axiom-0.1.5/axiom/drs/utilities.py`

 * *Files 3% similar despite different names*

```diff
@@ -460,15 +460,15 @@
 
     # Bail out if time-invariant
     if is_time_invariant(ds):
         return 'fx'
 
     # Take the difference between the first two time steps
     diff = (ds.time.data[1] - ds.time.data[0])
-    total_seconds =  pd.to_timedelta([diff]).astype('timedelta64[s]')[0].astype(np.int32)
+    total_seconds =  pd.to_timedelta([diff]).total_seconds()
 
     # TODO: These should be configurable
     intervals = '1H,3H,6H,1D,1M'.split(',')
     seconds = [
         1*60*60,
         3*60*60,
         6*60*60,
@@ -605,8 +605,33 @@
     # Filter for the variable name
     filtered_filepaths = list()
     for filepath in filepaths:
         filename = os.path.basename(filepath)
         if re.search(pattern, filename):
             filtered_filepaths.append(filepath)
     
-    return filtered_filepaths
+    return filtered_filepaths
+
+
+def get_start_and_end_dates(year, output_frequency):
+    """Get the start and end dates for interpolation context.
+
+    Args:
+        year (int): Current year
+        output_frequency (str): Frequency.
+    """
+    start_date = f'{year}0101' if output_frequency[-1] != 'M' else f'{year}01'
+    end_date = f'{year}1231' if output_frequency[-1] != 'M' else f'{year}12'
+    return start_date, end_date
+
+
+def generate_years_list(start_year, end_year):
+    """Generate a list of years (decades) to process.
+
+    Args:
+        start_year (int): Start year.
+        end_year (int): End year.
+
+    Returns:
+        iterator : Years to process.
+    """
+    return range(start_year, end_year+1, 10)
```

### Comparing `acs-axiom-0.1.4/axiom/drs.old.py` & `acs-axiom-0.1.5/axiom/drs.old.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/exceptions.py` & `acs-axiom-0.1.5/axiom/exceptions.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/qa/__init__.py` & `acs-axiom-0.1.5/axiom/qa/__init__.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/report.py` & `acs-axiom-0.1.5/axiom/report.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/schemas/__init__.py` & `acs-axiom-0.1.5/axiom/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/tests/data/mrd.xml` & `acs-axiom-0.1.5/axiom/tests/data/mrd.xml`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/tests/test_config.py` & `acs-axiom-0.1.5/axiom/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/tests/test_drs.py` & `acs-axiom-0.1.5/axiom/tests/test_drs.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/tests/test_drs_utilities.py` & `acs-axiom-0.1.5/axiom/tests/test_drs_utilities.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/tests/test_utilities.py` & `acs-axiom-0.1.5/axiom/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/utilities.py` & `acs-axiom-0.1.5/axiom/utilities.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/axiom/validation/validator.py` & `acs-axiom-0.1.5/axiom/validation/validator.py`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/bin/axiom` & `acs-axiom-0.1.5/bin/axiom`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/Makefile` & `acs-axiom-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/cli.rst.txt` & `acs-axiom-0.1.5/docs/source/cli.rst`

 * *Files 5% similar despite different names*

```diff
@@ -40,8 +40,14 @@
 Convert CORDEX
 --------------
 
 The ``convert_cordex`` subcommand will convert a CORDEX attribute CSV (from CCAM) into an Axiom schema.
 
 .. code-block:: shell
 
-    axiom convert_cordex codex_var_info_day.csv cordex-day.json
+    axiom convert_cordex codex_var_info_day.csv cordex-day.json
+
+
+DRS
+---
+
+See :ref:`DRS <drs>`
```

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/conversion.rst.txt` & `acs-axiom-0.1.5/docs/source/conversion.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/metadata.rst.txt` & `acs-axiom-0.1.5/docs/source/metadata.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/reporting.rst.txt` & `acs-axiom-0.1.5/docs/source/reporting.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     generate_report(
         validator, # A validator object that has been used.
         input_filepath, # The path to the original input file.
         report_filepath # The path to which to write the report
     )
 
 
-The report will be a plain text file:
+The report will be a plain text file in the following format:
 
 .. code-block:: text
 
     Axiom Validator 0.1.0
     Report generated: 2021-06-04 13:36:10.227704
     schema_filepath: specifications/mrd-0.1.0.json
     input_filepath: test.json
```

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/schemas.rst.txt` & `acs-axiom-0.1.5/docs/source/schemas/schemas.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-.. _schemas:
 Metadata Schemas
 ================
 
 A metadata schema (also referred to as a "specification") is a configuration file which defines the rules and standards that metadata must conform to in order to "meet the standard" and pass validation checks. They too are written as a JSON configuration file following a strict format and using validation rules defined by the Cerberus validation library, a subsystem used by Axiom.
 
 https://docs.python-cerberus.org/en/stable/index.html
 
@@ -55,14 +54,37 @@
                 "description": {"type": "string"}
             }
         }
     }
 
 Again, all attributes defined in a variable's schema are required by default.
 
+Default variable attribute
+--------------------------
+
+There is one special configuration option for variable schemas, the ``_default`` configuration option. If a schema provides a ``_default`` configuration option, it sets a base set of validation rules which all other variables inherit or override.
+
+For example:
+
+.. code-block:: json
+
+    {
+        "variables": {
+            "_default": {
+                "units" : {"type": "string"},
+                "description" : {"type": "string"},
+                "standard_name": {"type": "string"},
+                "long_name": {"type": "string"}
+            }
+        }
+    }
+
+
+This example will enforce all variables to require units, description, standard_name and long_name as metadata attributes, unless they provide their own set of rules.
+
 Putting it all together
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 Using the above examples, the complete metadata schema could take the following form:
 
 .. code-block:: json
```

### Comparing `acs-axiom-0.1.4/docs/build/html/_sources/validation.rst.txt` & `acs-axiom-0.1.5/docs/source/validation.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/make.bat` & `acs-axiom-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/source/axiom.drs.rst` & `acs-axiom-0.1.5/docs/source/axiom.drs.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/source/axiom.rst` & `acs-axiom-0.1.5/docs/source/axiom.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/source/conf.py` & `acs-axiom-0.1.5/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,28 @@
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
+from datetime import datetime
+from axiom import __version__
 sys.path.insert(0, os.path.abspath('../..'))
 
 
 # -- Project information -----------------------------------------------------
 
 project = 'Axiom'
-copyright = '2021, Ben Schroeter'
+year = datetime.utcnow().year
+copyright = f'{year}, Ben Schroeter'
 author = 'Ben Schroeter'
 
 # The full version, including alpha/beta/rc tags
-release = '0.0.1'
+release = __version__
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `acs-axiom-0.1.4/docs/source/custom_processors.rst` & `acs-axiom-0.1.5/docs/source/drs/custom_processors.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/source/installation.rst` & `acs-axiom-0.1.5/docs/source/installation.rst`

 * *Files 21% similar despite different names*

```diff
@@ -1,47 +1,38 @@
 Installation
 ============
 
 Axiom is installed via pip and should be installed inside a virtual environment such as conda.
 
-As the project matures, these steps will become more automated and familiar.
-
-Create environment
+Install Axiom from scratch.
 ------------------
 
 .. code-block:: shell
     
     # Create a conda environment
     conda create -n axiom_dev
     conda activate axiom_dev
 
+    # Install Axiom from pip
+    pip install acs-axiom
+
 
-Install Axiom
+Install Axiom on NCI
 -------------
 
 .. code-block:: shell
 
-    # Clone the repository
-    git clone git@github.com:AusClimateService/axiom.git
-
-    # Navigate to the local copy
-    cd axiom
-
-    # Install
-    pip install .
-
-    # Move back up
-    cd ..
+    # Select the hh5 modules
+    module use /g/data/hh5/public/modules
 
+    # Load the module
+    module load conda/analysis3
 
-Install Axiom Schemas
----------------------
-
-Most of the utilities dependencies will be installed automatically, with the exception of the Axiom Schemas component, which must be installed separately.
-
-.. code-block:: shell
+    # Create a virtual environment and activate it
+    conda create -n axiom_dev pip
+    conda activate axiom_dev
 
-    # Clone Axiom Schemas
-    git clone git@github.com:AusClimateService/axiom-schemas.git
+    # Install Axiom
+    pip install acs-axiom
 
-    cd axiom_schemas
-    pip install -e .    
+    # Alternatively, install to user space
+    pip install --user acs-axiom
```

### Comparing `acs-axiom-0.1.4/docs/source/performance.rst` & `acs-axiom-0.1.5/docs/source/drs/performance.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/docs/source/qa.rst` & `acs-axiom-0.1.5/docs/source/qa.rst`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/setup.cfg` & `acs-axiom-0.1.5/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 [options]
 packages = find:
 zip_safe = False
 scripts = bin/axiom
 include_package_data = True
 python_requires = >=3.11
 install_requires = 
-	xarray >= 2022.3.0
-	netCDF4 >= 1.5.8
-	h5netcdf >= 1.0.0
+	xarray >= 2023.5.0
+	netCDF4 >= 1.6.3
+	h5netcdf >= 1.1.0
 	cerberus >= 1.3.4
-	tabulate >= 0.8.9
-	dask >= 2022.8.1
-	distributed >= 2022.8.1
-	tqdm >= 4.64.1
+	tabulate >= 0.9.0
+	dask >= 2023.5.1
+	distributed >= 2023.5.1
+	tqdm >= 4.65.0
 	Jinja2 >= 3.1.2
 	importlib-metadata >= 6.6.0
 
 [aliases]
 test = pytest
 
 [tool:pytest]
```

### Comparing `acs-axiom-0.1.4/specifications/cf-77.json` & `acs-axiom-0.1.5/specifications/cf-77.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cf-standard-name-table.xml` & `acs-axiom-0.1.5/specifications/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex-day.json` & `acs-axiom-0.1.5/specifications/cordex-day.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex-fx.json` & `acs-axiom-0.1.5/specifications/cordex-fx.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex-month.json` & `acs-axiom-0.1.5/specifications/cordex-month.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex_var_info_day.csv` & `acs-axiom-0.1.5/specifications/cordex_var_info_day.csv`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex_var_info_fx.csv` & `acs-axiom-0.1.5/specifications/cordex_var_info_fx.csv`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/cordex_var_info_mon.csv` & `acs-axiom-0.1.5/specifications/cordex_var_info_mon.csv`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/mrd-0.1.0.json` & `acs-axiom-0.1.5/specifications/mrd-0.1.0.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/mrd-0.2.0.json` & `acs-axiom-0.1.5/specifications/mrd-0.2.0.json`

 * *Files identical despite different names*

### Comparing `acs-axiom-0.1.4/specifications/mrd.xsd` & `acs-axiom-0.1.5/specifications/mrd.xsd`

 * *Files identical despite different names*

